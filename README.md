# Monitor

[![GPL-3.0](https://img.shields.io/github/license/auto-novel/monitor)](https://github.com/auto-novel/monitor#license)

## 功能

- [**node**](https://github.com/prometheus/node_exporter): 用于采集*NIX内核暴露的硬件与操作系统指标
- [**cadvisor**](https://github.com/google/cadvisor): 用于采集运行中容器的资源使用情况和性能特征
- [**sakura_share**]: 用于采集 Sakura Share 服务的性能指标

## 部署

下载项目：

```bash
> git clone https://github.com/auto-novel/monitor.git
> cd monitor
```

创建并编辑 `.env` 文件，内容如下:

```bash
GF_SERVER_ROOT_URL=             # Monitor 挂载的 url
GF_SECURITY_ADMIN_USER=         # 管理员用户名
GF_SECURITY_ADMIN_PASSWORD=     # 管理员密码
```

运行 `docker compose up -d` 命令启动服务。
