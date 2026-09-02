# Windows 发布目录

这里记录 GuGu Pet Host 的 Windows x64 安装包，以及 Windows 专用的 GPT-SoVITS V2/V4 独立能力包约定。大文件作为 GitHub Release 资产发布，不提交到 Git 历史。

## 主应用

- Release：[`v0.1.0-beta.7`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.7)
- 安装器：`GuGu.Pet.Host-0.1.0-beta.7-x64.exe`
- 校验：同名 `.sha256` 资产，安装前请核对 SHA-256。
- 支持：Windows 10/11 x64。

主应用是纯净安装包：不含任何开发者 API Key、测试账号、聊天记录，也不含 GPT-SoVITS 的 Python 运行时、引擎代码或模型权重。宠物、Live2D 和本地识别资源按内测授权随应用提供。

## GPT-SoVITS 独立能力包

Windows GPT-SoVITS 独立包请使用 [`v0.1.0-windows`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-windows) Release；macOS 的 `v0.1.0` Release 不适用于 Windows。

V2 与 V4 必须分别下载，不能互换。能力包不在主应用安装目录中，安装位置由应用自动管理：

```text
%APPDATA%\desktop-pet-host\voice-engine-packs\
  guga-gpt-sovits-v2-win32-x64.zip
  guga-gpt-sovits-v4-win32-x64.zip
```

用户只需把对应 ZIP 及其 `.zip.000`、`.zip.001` 分片原样放入上述目录，然后在“设置 → 扩展与连接 → GPT-SoVITS”选择 V2 或 V4 并点击安装。应用会合并、校验、安装和启动已调试的运行时，不要求用户自行安装 Python、Conda、端口或调试服务。Windows V2/V4 独立包发布后会在对应引擎 Release 中提供直达链接；主应用安装器永远不包含这些引擎。

## 功能边界

PPT 工作台暂不对用户开放。安装后点击任何“打开 PPT 工作台”入口，应用只显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。
