# YuanMind 下载仓库

这是 YuanMind 的公开安装包下载仓库。

本仓库只用于：

- 发布安装包
- 维护版本说明
- 提供校验和
- 说明安装步骤

本仓库不包含 YuanMind 产品源码。YuanMind 源码仓库保持私有。

## 最新版本

安装包会发布在 GitHub Releases：

```txt
https://github.com/lihuan6015-droid/yuanmind-downloads/releases/latest
```

当前阶段：安装包尚未上传。内测早期安装包可能尚未完成正式签名、公证或 Windows 代码签名；下载前请优先确认 Release 来源和 SHA-256 校验和。

## 平台状态

| 平台 | 状态 |
|---|---|
| macOS | 内测优先，等待签名/公证/真机验收后上传 |
| Windows | 等待打包验收 |
| Linux | 规划中 |

## 安装说明

> 未签名内测包只建议在你信任 YuanMind 发布来源、且校验和一致时安装。不要从第三方转发链接下载安装包。

### macOS

1. 从 Releases 下载 `.dmg` 安装包。
2. 打开 `.dmg`。
3. 将 YuanMind 拖入 Applications。
4. 首次启动如遇 “无法打开，因为无法验证开发者” 或类似 Gatekeeper 提示：
   - 推荐方式：在 Finder 中右键 YuanMind，选择“打开”，再在系统提示中确认打开。
   - 或者：先尝试打开一次失败后，进入“系统设置 → 隐私与安全性”，在安全提示处选择“仍要打开”。
5. 如果内测包仍被 quarantine 标记拦截，且你已确认校验和无误，可在终端执行：

```bash
xattr -dr com.apple.quarantine /Applications/YuanMind.app
```

不建议关闭 Gatekeeper 全局安全策略。

### Windows

1. 从 Releases 下载 `.exe` 安装包。
2. 双击运行安装程序。
3. 如果 Windows SmartScreen 提示“Windows 已保护你的电脑”，请先确认文件来自本仓库 Release 且校验和一致，再选择“更多信息 → 仍要运行”。
4. 如果文件属性中出现“此文件来自其他计算机，可能被阻止”，可右键安装包 → “属性” → 勾选“解除锁定” → 应用。

不建议关闭 Windows Defender 或系统安全防护来安装内测包。

## 校验和

每个正式 Release 都应附带 SHA-256 校验和。上传安装包后，请同步更新：

```txt
checksums/SHA256SUMS.txt
```

## 公开下载说明

本仓库是公开仓库，外部人员可以下载安装包。公开下载安装包不代表 YuanMind 开源。
