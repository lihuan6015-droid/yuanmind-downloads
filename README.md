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

当前阶段：安装包尚未上传。请等待 macOS / Windows 安装包完成签名、公证、打包和真机验收。

## 平台状态

| 平台 | 状态 |
|---|---|
| macOS | 内测优先，等待签名/公证/真机验收后上传 |
| Windows | 等待打包验收 |
| Linux | 规划中 |

## 安装说明

### macOS

1. 从 Releases 下载 `.dmg` 安装包。
2. 打开 `.dmg`。
3. 将 YuanMind 拖入 Applications。
4. 首次启动如遇 macOS 安全提示，请按正式版本说明操作。

### Windows

1. 从 Releases 下载 `.exe` 安装包。
2. 双击运行安装程序。
3. 如遇安全软件提示，请确认文件来自本仓库正式 Release。

## 校验和

每个正式 Release 都应附带 SHA-256 校验和。上传安装包后，请同步更新：

```txt
checksums/SHA256SUMS.txt
```

## 公开下载说明

本仓库是公开仓库，外部人员可以下载安装包。公开下载安装包不代表 YuanMind 开源。
