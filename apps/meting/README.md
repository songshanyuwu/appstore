# Meting

## 简介
Meting 是一个开源的音乐 API 服务。

## 安装步骤
1. 确保已经安装并配置好 Docker 和 1Panel。
2. 按照提示填写相关配置参数并完成安装。
3. 反向代理时添加如下内容
```
location /meting/ {
    proxy_pass http://localhost:3000/;
    proxy_set_header X-Forwarded-Host $scheme://$host:$server_port/meting;
}
```

## 升级
- 目前没有升级脚本，直接重新部署最新版本即可。

## 卸载
- 删除 Docker 容器和相关数据即可。

## 文档
- 详细使用文档请参考 [官方文档](https://github.com/xizeyoupan/Meting-API)。
