# Caddy Custom Build

通过 GitHub Actions 自动编译含 DNS 插件的 Caddy 二进制。

- 每周日 03:00 UTC 定时编译（amd64 + arm64）
- 支持手动触发指定版本和额外模块
- 手动触发时创建 GitHub Release
