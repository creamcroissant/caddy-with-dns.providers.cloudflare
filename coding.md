# 开发记录

## 2026-06-22 创建 GitHub Actions 自动编译 Caddy

- **目标**: 定时编译含 `dns.providers.cloudflare` 模块的 Caddy 二进制
- **文件**: `.github/workflows/build-caddy.yml`
- **功能**:
  - 每周日凌晨 3:00 UTC 自动编译
  - 支持手动触发（可指定 Caddy 版本和额外模块）
  - linux/amd64 + linux/arm64 双架构
  - 自动上传 Artifact，手动触发时创建 GitHub Release
- **参考**: 博客仅摘取编译命令 `xcaddy build --with github.com/caddy-dns/cloudflare`，部署步骤不纳入
