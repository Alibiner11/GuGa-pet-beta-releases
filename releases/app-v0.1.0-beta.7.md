# GuGu Pet Host macOS 内测版 v0.1.0-beta.7

面向受邀的 macOS Apple Silicon（M 系列芯片、arm64）测试用户。本次为最新 macOS 内测构建，对应项目提交 `2203cd2`。

## 下载与校验

从 [`v0.1.0-beta.7`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.7) 下载：

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.7-arm64.dmg` | macOS Apple Silicon 安装包 | `a3fc782a5c24fbbe85176c7209ab744305f84cb34ad189898cecc1686199a2ec` |

终端校验：

```bash
shasum -a 256 GuGu.Pet.Host-0.1.0-beta.7-arm64.dmg
```

## 安装与已知边界

打开 DMG 后，将 `GuGu Pet Host.app` 拖入“应用程序”。本安装包未进行 Apple 开发者签名或公证；请确认下载来源为本仓库，首次打开时可通过 Finder 右键应用并选择“打开”。

PPT 工作台暂不开放。点击入口只会显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。

主安装包不包含 GPT-SoVITS 音色克隆的运行时或模型权重。macOS 用户应在“设置 → 扩展与连接”按需安装独立引擎包，并优先选择 V2；V4 会占用更多系统资源，可能造成设备性能下降、语音合成速度明显变慢，仅建议在有专门测试需求时试用。

本版本仅限受邀测试、体验和反馈，不可用于商业销售、收费服务、公开再分发、反向工程或单独提取/传播包内受保护资源。安装包不包含开发者 API Key、测试账号或用户数据；Live2D 和其他第三方资源继续受各自许可约束。
