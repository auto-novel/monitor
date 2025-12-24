# Monitor 监控服务

[![GPL-3.0](https://img.shields.io/github/license/auto-novel/monitor)](https://github.com/auto-novel/monitor#license)

该项目是网站内部基础设施与服务的性能监控系统，用于跟踪和可视化关键指标。

- [机翻站数据看板](http://monitor.novelia.cc/public-dashboards/3744e66a0c374631b7556b95a7eb40a7)
- [Sakura Share数据看板](http://monitor.novelia.cc/public-dashboards/be71c46fcc0e40eeaf06d9e7a2e26f95)

## 部署

```bash
# 1. 克隆仓库
git clone https://github.com/auto-novel/monitor.git
cd monitor

# 2. 生成环境变量配置
cat > .env << EOF
GF_SERVER_ROOT_URL=%(protocol)s://monitor.novelia.cc
GF_SECURITY_ADMIN_USER=     # 管理员用户名
GF_SECURITY_ADMIN_PASSWORD= # 管理员密码
EOF

# 3. 启动服务
docker compose up -d
```
