# Windows 10/11 x64 下载与安装

本页只适用于 Intel / AMD 64 位 Windows 10/11（`win32-x64`）。Windows on ARM、32 位 Windows 和 macOS 都不适用；请勿下载或混用 macOS `darwin-arm64` 文件。

## 1. 安装 GuGu Pet Host

下载 [beta.7 Windows 安装器（EXE）](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.7/GuGu.Pet.Host-0.1.0-beta.7-x64.exe)，并用 [SHA-256 文件](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.7/GuGu.Pet.Host-0.1.0-beta.7-x64.exe.sha256) 校验。运行 EXE 完成安装。

## 2. 按需安装 GPT-SoVITS 音色克隆包

音色克隆包不在主安装器内。每个版本都必须下载该行的**所有分片和校验文件**，原样放入 `%APPDATA%\desktop-pet-host\voice-engine-packs\`；不要改名、提前解压或混用 V2/V4 分片。之后在“设置 → 扩展与连接 → GPT-SoVITS”选择对应版本并点击安装。

| 版本 | 分片 | 校验文件 |
| --- | --- | --- |
| V2 | [`.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v2-win32-x64.zip.000) · [`.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v2-win32-x64.zip.001) · [`.002`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v2-win32-x64.zip.002) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v2-win32-x64.zip.sha256) |
| V4 | [`.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v4-win32-x64.zip.000) · [`.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v4-win32-x64.zip.001) · [`.002`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v4-win32-x64.zip.002) · [`.003`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v4-win32-x64.zip.003) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-windows/guga-gpt-sovits-v4-win32-x64.zip.sha256) |

主安装器和能力包不包含任何开发者 API Key、测试账号或用户数据。PPT 工作台暂不对用户开放；点击入口只显示“PPT 工作台还在完善中，敬请等待后续更新”。
