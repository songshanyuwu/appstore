# PlayEdu开源培训系统

![](https://meedu.cloud.oss.meedu.vip/playedu/%E5%A4%B4%E5%9B%BE.jpg)

PlayEdu 是由白书科技团队经营多年线上教育系统打造出的一款全新的企业培训方案，致力于为更多企业机构搭建私有化内部培训平台。
PlayEdu 基于 Java + MySQL 开发，采用前后端分离模式，前台采用 React18 为核心框架，后台采用 SpringBoot3 为核心框架。

## 系统演示

| -            | 站点                                                   | 账号                | 密码     |
| ------------ | ------------------------------------------------------ | ------------------- | -------- |
| 后台管理端口 | [https://admin.playedu.xyz](https://admin.playedu.xyz) | `admin@playedu.xyz` | `123123` / `playeedu` |
| 学员端口     | [https://demo.playedu.xyz](https://demo.playedu.xyz)   | `1@playedu.xyz`     | `123123` / `自行创建` |
| H5端演示(移动端访问) | [https://h5.playedu.xyz](https://h5.playedu.xyz) | `1@playedu.xyz` | `123123` / `自行创建`  |

如果尝试密码错误多次被锁定60分钟，可以尝试重启Redis。

## 快速开始(一键部署)

自动挡 - 使用 docker-compose 安装(https://www.playedu.xyz/docs/docs/install/role-docker/docker-compose)

[Github地址](https://github.com/PlayEdu/PlayEdu)
[Gitee地址](https://gitee.com/playeduxyz/playedu)

### MinIO配置

登录进入到后台，选择系统配置 - MinIO 配置，按照下面的表格输入对应的配置：

| 配置项 | 	需要配置的值|
| --------- | -------------------------| 
| AccessKey | username         |
| SecretKey | password         |
|  Bucket   | playedu        |
|  Endpoint | http://你的服务器IP:9002 |
|  Domain   | http://你的服务器IP:9002 |

保存配置。到这里，安装全部完成。

## 使用协议

● 要求
- 保留页脚处版权信息。
- 保留源代码中的协议。
- 如果修改了代码，则必须在文件中进行说明。

● 允许
- 私用、商用、修改。

## 官方交流群

<p><img src="https://meedu.cloud.oss.meedu.vip/playedu/PlayEduk%E5%AE%A2%E6%9C%8D-zhu.png" width="200" /></p>