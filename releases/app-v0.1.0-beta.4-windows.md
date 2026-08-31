# GuGu Pet Host Windows 内测版 v0.1.0-beta.4

面向受邀 Windows 10/11 x64 测试用户。本版本包含 beta.4 主应用更新，不改变语音克隆能力包的独立发布方式。

## 下载与校验

从 [`v0.1.0-beta.4`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.4) 下载：

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.4-x64.exe` | Windows x64 安装器 | `9b428b21c4f4ec0ea042f004128402b23b0d63ac3cb0686ba167cc0ac192f12a` |
| `GuGu.Pet.Host-0.1.0-beta.4-x64.exe.blockmap` | 增量更新元数据 | `92953a349065ab6d42011eda61ecdac4ec1aa9a35a5fb2dba7d68666b043b6b4` |

PowerShell 校验：

```powershell
Get-FileHash .\GuGu.Pet.Host-0.1.0-beta.4-x64.exe -Algorithm SHA256
```

## 安装与边界

运行安装器完成安装。首次启动后在“设置 → 模型与 API”填写用户自己的服务配置；安装包不包含开发者 API Key、测试账号或用户数据。

GPT-SoVITS V2/V4 不在主安装器内。需要音色克隆时，请按 [`Windows 发布目录说明`](./windows/README.md) 下载对应的独立能力包，应用会自动安装、连接和启动。

PPT 工作台暂不开放。点击入口只显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。
