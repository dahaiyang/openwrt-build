# OpenWRT 云编译 - 京东云 ER1 (RE-CS-07)

高通 IPQ60XX 平台专用固件编译配置

## 📋 设备信息

- **设备**: 京东云 ER1 (RE-CS-07)
- **平台**: 高通 IPQ6000/6010
- **存储**: 256MB NAND
- **内存**: 512MB RAM
- **源码**: [VIKINGYFY/immortalwrt](https://github.com/VIKINGYFY/immortalwrt) (高通专用版)

## 🚀 快速开始

### 1. 手动触发编译

1. 进入 GitHub 仓库 → Actions
2. 选择 **JDC-ER1-Build**
3. 点击 **Run workflow**
4. 等待 1-3 小时完成

### 2. 定时自动编译

默认每天早上 4 点（北京时间）自动编译，可在 `.github/workflows/JDC-ER1-Build.yml` 中修改或关闭。

## 📦 包含的插件

### 科学上网
- HomeProxy (sing-box)
- Passwall (完整版)
- OpenClash
- SSR-Plus
- Hysteria / Tuic / NaiveProxy
- Shadowsocks-Rust
- Xray-core / V2ray

### 网络工具
- DDNS
- Tailscale
- FRP 内网穿透
- Cloudflared Tunnel
- UPnP
- SQM QoS (NSS 加速)

### 系统工具
- TTYD Web 终端
- Filebrowser 文件管理
- Samba4 文件共享
- USB 打印
- 自动重启

### 其他
- Adblock 广告拦截
- 解锁网易云音乐
- KMS 激活服务

## ⚙️ 默认配置

- **IP 地址**: 192.168.10.1
- **主机名**: JDC-ER1
- **主题**: Aurora
- **WiFi**: 无（ER1 无无线功能）

## 📥 固件下载

编译完成后，在 Actions 页面下载Artifacts，或查看 Releases 页面。

## ⚠️ 注意事项

1. **首次刷机**请使用 factory 固件
2. **升级**使用 sysupgrade 固件
3. 刷机前请备份配置

## 🔧 故障排除

如果编译失败，可能是：
- GitHub Actions 磁盘空间不足（已优化清理）
- 内存不足（已添加 swap）
- 源码更新导致不兼容

可尝试重新运行 workflow。

## 📄 许可证

遵循 ImmortalWrt 开源许可证
