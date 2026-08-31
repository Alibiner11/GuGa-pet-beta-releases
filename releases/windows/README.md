# GuGu Pet Windows 发布说明

## 主应用

当前最新 Windows 安装包为 [`v0.1.0-beta.4`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.4)，仅支持 Windows 10/11 x64。

- [下载 Windows x64 安装器](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-x64.exe)
- [下载 SHA-256 校验文件](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.4/GuGu.Pet.Host-0.1.0-beta.4-x64.exe.sha256)

主应用是纯净安装包：不包含开发者 API Key、测试账号、聊天记录，也不包含 GPT-SoVITS 的 Python 运行时、引擎代码或模型权重。宠物、Live2D 和本地识别资源按内测授权随应用提供。

PowerShell 校验示例：

```powershell
Get-FileHash .\GuGu.Pet.Host-0.1.0-beta.4-x64.exe -Algorithm SHA256
```

## GPT-SoVITS 独立能力包

V2 与 V4 必须分别下载，不能互换。能力包不在主应用安装目录中，安装位置由应用自动管理：

```text
%APPDATA%\desktop-pet-host\voice-engine-packs\
  guga-gpt-sovits-v2-win32-x64.zip
  guga-gpt-sovits-v4-win32-x64.zip
```

用户只需把对应 ZIP 及其 `.zip.000`、`.zip.001` 分片原样放入上述目录，然后在“设置 → 扩展与连接 → GPT-SoVITS”选择 V2 或 V4 并点击安装。应用会合并、校验、安装和启动已调试的运行时，不要求用户自行安装 Python、Conda、端口或调试服务。两个版本的独立包和 `.sha256` 校验文件发布在 [`v0.1.0`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0)；Windows 包资产准备完成后会追加到该 Release。

## 功能边界

PPT 工作台暂不对用户开放。安装后点击任何“打开 PPT 工作台”入口，应用只显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。
