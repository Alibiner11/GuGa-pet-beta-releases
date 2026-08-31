# GuGu Pet Host Windows 内测版 v0.1.0-beta.3

面向受邀 Windows 10/11 x64 测试用户。

## 下载与校验

从 [`v0.1.0-beta.3`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.3) 下载：

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.3-x64.exe` | Windows x64 安装器 | `24c2590dcfaaae4216fe5cfe1867310237434f62b4dccb8eedeb0f1d9424a0c5` |
| `GuGu.Pet.Host-0.1.0-beta.3-x64.exe.blockmap` | 增量更新元数据 | `bf13189525939154d8c8dea97be13291a57279147074cdcf318d6409b92ea70e` |

PowerShell 校验命令：

```powershell
Get-FileHash .\GuGu.Pet.Host-0.1.0-beta.3-x64.exe -Algorithm SHA256
```

## 安装

运行安装器并按向导完成安装。首次启动后在“设置 → 模型与 API”中填写用户自己的服务配置；安装包不会预置 API Key 或测试账号。

GPT-SoVITS 不在安装器内。需要音色克隆时，请按 [`Windows 发布目录说明`](./windows/README.md) 下载并导入 V2 或 V4 独立能力包。

PPT 工作台当前锁定；点击入口会提示功能正在完善中，请耐心等待后续更新。
