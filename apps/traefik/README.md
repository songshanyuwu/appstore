# Traefik

[WIP]

Traefik在1Panel中使用的共享网络是1panel-network

## 推荐附加配置

### 自动生成泛域名证书 Labels

使用前确保已经完成 `Let's Encrypt` 的配置

```yaml
labels:
    traefik.enable: true
    traefik.http.routers.traefik.rule: Host("traefik.example.com")
    traefik.http.routers.traefik.entrypoints: http
    traefik.http.routers.traefik.tls.certresolver: myresolver
    traefik.http.routers.traefik.tls.domains[0].main: example.com
    traefik.http.routers.traefik.tls.domains[0].sans: example.com,*.example.com
    traefik.http.services.traefik.loadbalancer.server.port: 8080
```

## 常用代理配置

```yaml
traefik.enable: true
traefik.docker.network: traefik
traefik.http.routers.rsc-https.rule: Host("<host>")
traefik.http.routers.rsc-https.entrypoints: https,proxys
traefik.http.routers.rsc-https.tls.certresolver: myresolver
traefik.http.services.rsc.loadbalancer.server.port: <port>
```