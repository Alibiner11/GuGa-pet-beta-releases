# GuGu Pet Host macOS 内测版 v0.1.0-beta.4

这是面向受邀测试用户的 macOS Apple Silicon（M 系列芯片、arm64）安装包；Intel Mac、Windows 和 Linux 不适用本文件。

## 本次更新

- 桌面宠物支持停靠屏幕边缘并折叠为把手，且仅在宠物本体真正越出屏幕时触发折叠。
- 头像支持由用户框选，安静模式会展示已选择的头像结果。
- 优化聊天文件结果卡片与轻量计划中的重命名参数处理。
- PPT 工作台继续保持内测锁定；点击入口只会提示功能仍在完善中，不会打开工作台或调用相关能力。

## 下载与校验

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.4-arm64.dmg` | macOS Apple Silicon 安装包 | `dc6c91b8df09bad1100d34af33450c595fc75604f8d966161789789288a14c98` |
| `GuGu.Pet.Host-0.1.0-beta.4-arm64.dmg.sha256` | 完整性校验文件 | 与上列 DMG 对应 |

在 macOS 终端中可运行：

```bash
shasum -a 256 "GuGu.Pet.Host-0.1.0-beta.4-arm64.dmg"
```

输出应与上表一致。

## 安装与使用

1. 确认设备为 Apple Silicon（M 系列芯片）Mac。
2. 打开 DMG，将应用拖到“应用程序”目录。
3. 安装前阅读 DMG 根目录的“内测说明.md”。
4. 首次运行后进入“设置 → 模型与 API”，配置自己的 API Key、模型与第三方服务。

本构建未使用 Apple 开发者签名/公证。若 macOS 阻止首次启动，请确认下载来源后在 Finder 中右键应用并选择“打开”。

## 内测与资源边界

本版本仅限受邀测试、体验和反馈，不能用于商业销售、收费服务、公开再分发、反向工程或单独提取/传播包内受保护资源。Live2D 和其他第三方资源仍受各自许可约束；详情见仓库的 [内测范围与资源说明](https://github.com/Alibiner11/GuGu-pet-beta-releases/blob/main/INTERNAL_BETA_SCOPE.md)。
