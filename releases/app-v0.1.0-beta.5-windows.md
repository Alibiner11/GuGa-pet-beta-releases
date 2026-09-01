# GuGu Pet Host Windows 内测版 v0.1.0-beta.5

面向受邀 Windows 10/11 x64 测试用户。本版本对应项目提交 `eee130e` 之后的最新构建。

## 下载与校验

从 [`v0.1.0-beta.5`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.5) 下载：

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.5-x64.exe` | Windows x64 安装器 | `D7EAE1CBB9FEB3DDC263405D460EF8AC64C97A88C1A383262AD54C4C5A1EE815` |
| `GuGu.Pet.Host-0.1.0-beta.5-x64.exe.blockmap` | 增量更新元数据 | `6368EA1F97DB8E746D4EF60D2227DD35FA288BCAB0D6B2A6D45E108A7B515D8E` |

PowerShell 校验：

```powershell
Get-FileHash .\GuGu.Pet.Host-0.1.0-beta.5-x64.exe -Algorithm SHA256
```

## 安装与边界

运行安装器完成安装。首次启动后在“设置 → 模型与 API”填写用户自己的服务配置；安装包不包含开发者 API Key、测试账号或用户数据，也不包含 GPT-SoVITS 运行时和模型权重。宠物与内测所需资源随主应用提供。

GPT-SoVITS V2/V4 不在主安装器内，分别作为独立能力包发布。请按 [`Windows 发布目录说明`](./windows/README.md) 下载对应版本，原样放入应用提示的 `voice-engine-packs` 目录后安装。

PPT 工作台暂不开放。点击入口只显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。
