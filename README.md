# WisPod Desktop Releases

WisPod 桌面端 release artifacts 的公开镜像。

## 说明

- 这个仓库**只放 release 文件**,源码不在这里
- 由 [Jimoulvdong/WhisPod](https://github.com/Jimoulvdong/WhisPod) 主仓 CI 自动同步
- 用途:作为 Tauri auto-updater 的 fallback endpoint(主端点 `https://wispod.ai/api/updater` 不可达时自动回退到这里)

## 自动更新协议

每个 release 都包含 `latest.json` 自动更新清单:

```
https://github.com/Jimoulvdong/WisPod-desktop-releases/releases/latest/download/latest.json
```

artifacts 经 minisign 签名,客户端用内置 pubkey 校验。

## 直接下载

如果想手动安装,直接到 [Releases](https://github.com/Jimoulvdong/WisPod-desktop-releases/releases) 取最新 `.dmg`。
