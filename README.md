# GuGu Pet Beta Releases

GuGu Pet 的公开内测发布仓库。这里仅发布可安装的内测应用、独立能力包及校验文件；不包含项目源码、开发机配置、API Key、测试账号、聊天记录或其他用户数据。

## 立即下载

请选择与设备匹配的安装包。当前最新版本为 `v0.1.0-beta.4`。

| 平台 | 适用设备 | 直达下载 | 校验文件 |
| --- | --- | --- | --- |
| Windows 10/11 x64 | 常见的 Intel / AMD 64 位 Windows 电脑 | [下载 Windows 安装器（.exe）](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-x64.exe) | [SHA-256](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-x64.exe.sha256) |
| macOS Apple Silicon（arm64） | M1、M2、M3、M4 及后续 M 系列芯片 Mac | [下载 macOS 安装包（.dmg）](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-arm64.dmg) | [SHA-256](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-arm64.dmg.sha256) |

Intel Mac、Windows on ARM、Windows 32 位和 Linux 目前没有对应安装包。所有历史版本和说明可在 [Releases](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases) 查看。

## 安装与首次使用

### Windows 10/11 x64

1. 下载并运行上方的 `.exe` 安装器。
2. 若系统出现未知发布者提示，请确认下载来源为本仓库后再继续；当前内测包尚未进行代码签名。
3. 首次启动后，前往“设置 → 模型与 API”，填写并管理自己的 API、模型或第三方服务配置。

### macOS Apple Silicon

1. 确认设备使用 M 系列芯片；本 DMG 不适用于 Intel Mac。
2. 打开 DMG，将 `GuGu Pet Host.app` 拖入“应用程序”。
3. 若 macOS 阻止首次启动，请确认下载来源后，在 Finder 中右键应用并选择“打开”。

安装包不预置开发者 API Key、测试账号或用户数据。安装前请阅读包内的“内测说明.md”。

## 当前内测状态

GuGu Pet 仍处于持续完善的邀请制内测阶段。当前版本重点验证跨平台桌宠体验、对话和任务协作、形象与交互呈现，以及用户自管模型配置下的稳定性。

已经随包交付的能力包括：

- 桌宠陪伴、对话、任务进度与待授权操作的呈现；
- Windows 和 macOS Apple Silicon 的主应用安装包；
- Live2D 测试形象、本地语音/识别等用于内测验证的运行资源；
- 可由用户自行配置和管理的模型与第三方服务连接。

### 当前暂不开放

**PPT 工作台仍在完善中，当前内测版不会开放。** 点击任何 PPT 工作台入口只会显示等待后续更新的提示，不会打开工作台，也不会调用相关模型能力或产生此项功能的使用成本。

GPT-SoVITS 音色克隆能力以独立包形式提供，不随主安装器重复捆绑。Windows 主应用暂不包含其运行时或模型权重；详见 [Windows 发布说明](./releases/windows/README.md)。

## 接下来的方向

内测的目的不是仓促扩展功能，而是先把日常使用中最重要的体验打磨稳定。接下来会围绕以下方向持续迭代：

- 提升 Windows 与 macOS 的安装、更新、兼容性和故障反馈体验；
- 继续改善桌宠交互、角色形象、对话和任务协作的连贯性；
- 在成本、稳定性和权限边界满足要求后，再以独立版本逐步开放 PPT 工作台；
- 逐步完善本地能力包、资源许可核验、诊断信息和发布流程，让测试反馈能更快转化为可靠更新。

这些是当前规划方向，不代表功能、时间或平台支持的承诺。每次开放范围会以对应 Release 说明为准。

## 反馈、商业与资源边界

请在提交反馈时附上系统版本、芯片或 CPU 类型、应用版本、复现步骤和已脱敏日志；不要公开 API Key、令牌、聊天内容或个人资料。

本仓库的安装包仅供受邀测试、体验和反馈。不得用于商业销售、收费服务、公开二次分发、品牌背书、反向工程、拆分提取或将包内受保护资源用于内测体验与反馈以外的用途。GuGu 项目原创代码、名称、标识、界面和原创素材的权利归相应权利人所有；第三方软件、模型、字体和素材继续受各自许可约束。

Live2D 及其他第三方资源只为当前内测验证保留；使用或公开商业化前须完成相应许可核验。完整范围、第三方资源说明与权利反馈流程请见 [内测范围与资源说明](./INTERNAL_BETA_SCOPE.md)。
