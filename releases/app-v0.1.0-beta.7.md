# GuGu Pet Host 跨平台内测版 v0.1.0-beta.7

面向受邀测试用户的当前跨平台内测构建，对应项目提交 `2203cd2`。请严格按设备平台下载对应安装包：macOS 与 Windows 不能混用。

## 下载与校验

从 [`v0.1.0-beta.7`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/tag/v0.1.0-beta.7) 下载：

| 文件 | 用途 | SHA-256 |
| --- | --- | --- |
| `GuGu.Pet.Host-0.1.0-beta.7-arm64.dmg` | macOS Apple Silicon（M 系列芯片）安装包 | `a3fc782a5c24fbbe85176c7209ab744305f84cb34ad189898cecc1686199a2ec` |
| `GuGu.Pet.Host-0.1.0-beta.7-x64.exe` | Windows 10/11 x64 安装器 | `1643c14bf366931b48426f82acaaf16ca7b6a638421ffd3411703a1a19d0e8dd` |

终端校验：

```bash
shasum -a 256 GuGu.Pet.Host-0.1.0-beta.7-arm64.dmg
```

## 按平台安装

### macOS Apple Silicon（arm64）

仅限 M 系列芯片 Mac。打开 DMG 后，将 `GuGu Pet Host.app` 拖入“应用程序”。本安装包未进行 Apple 开发者签名或公证；请确认下载来源为本仓库，首次打开时可通过 Finder 右键应用并选择“打开”。

### Windows 10/11（x64）

仅限 Intel / AMD 64 位 Windows。运行 EXE 安装器完成安装；Windows on ARM 与 32 位 Windows 不适用。可使用 PowerShell 执行 `Get-FileHash .\GuGu.Pet.Host-0.1.0-beta.7-x64.exe -Algorithm SHA256` 校验下载完整性。

## 共同的内测边界

PPT 工作台暂不开放。点击入口只会显示“PPT 工作台还在完善中，敬请等待后续更新”，不会打开工作台或调用 PPT 能力。

两个主安装包均不包含 GPT-SoVITS 音色克隆的运行时或模型权重。当前公开引擎包仅支持 macOS Apple Silicon；macOS 用户应在“设置 → 扩展与连接”按需安装并优先选择 V2。V4 会占用更多系统资源，可能造成设备性能下降、语音合成速度明显变慢，仅建议在有专门测试需求时试用。Windows 用户请勿导入 macOS 的 `darwin-arm64` 引擎包。

本版本仅限受邀测试、体验和反馈，不可用于商业销售、收费服务、公开再分发、反向工程或单独提取/传播包内受保护资源。安装包不包含开发者 API Key、测试账号或用户数据；Live2D 和其他第三方资源继续受各自许可约束。
