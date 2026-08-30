# GuGu Pet Host macOS 内测版 v0.1.0-beta.2

面向受邀 Apple Silicon（M 系列芯片）测试用户的 GuGu Pet Host 内测安装包。

## 本次更新

- PPT 工作台在当前内测阶段暂不开放；点击入口会提示功能仍在完善中，不会打开工作台或调用其相关能力。
- Live2D 测试模型补充开源来源、仅限内测使用且不可商用的提示。
- 应用、安装包与公开发布仓库统一更名为 GuGu Pet。

## 下载与校验

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.2-arm64.dmg` | macOS 安装包 | `58ca1e88e125ea18bbd299afb9b9d7d2c4531f92a2d483e70fc1bfc8e6d3dae1` |
| `GuGu.Pet.Host-0.1.0-beta.2-arm64.dmg.sha256` | 完整性校验文件 | 与上列 DMG 对应 |

在 macOS 终端中可运行：

```bash
shasum -a 256 "GuGu.Pet.Host-0.1.0-beta.2-arm64.dmg"
```

输出应与上表一致。

## 安装与使用

1. 打开 DMG，将应用拖到“应用程序”目录。
2. 安装前阅读 DMG 根目录的“内测说明.md”。
3. 首次运行后进入“设置 → 模型与 API”，配置自己的 API Key、模型与第三方服务。
4. 需要音色克隆时，在“扩展与连接”选择 GPT-SoVITS V4（推荐）或 V2，应用会从 `v0.1.0` 引擎 Release 自动安装。

本构建未使用 Apple 开发者签名/公证。若 macOS 阻止首次启动，请确认下载来源后在 Finder 中右键应用并选择“打开”。

## 内测与资源边界

本版本仅限受邀测试、体验和反馈，不能用于商业销售、收费服务、公开再分发、反向工程或单独提取/传播包内受保护资源。Live2D 和其他第三方资源仍受各自许可约束；详情见仓库的 [内测范围与资源说明](https://github.com/Alibiner11/GuGu-pet-beta-releases/blob/main/INTERNAL_BETA_SCOPE.md)。
