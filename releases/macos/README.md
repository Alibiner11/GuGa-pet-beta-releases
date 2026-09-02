# macOS Apple Silicon 下载与安装

本页只适用于 M1、M2、M3、M4 及后续 M 系列芯片 Mac（`darwin-arm64`）。Intel Mac 不适用；请勿下载 Windows `win32-x64` 文件。

## 1. 安装 GuGu Pet Host

下载 [beta.8 macOS 安装包（DMG）](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.8-macos-arm64/GuGu.Pet.Host-0.1.0-beta.8-arm64.dmg)，并用 [SHA-256 文件](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0-beta.8-macos-arm64/GuGu.Pet.Host-0.1.0-beta.8-arm64.dmg.sha256) 校验。打开 DMG 后，将 `GuGu Pet Host.app` 拖入“应用程序”。

## 2. 按需安装 GPT-SoVITS 音色克隆包

音色克隆包不在主安装器内。每个版本都必须下载该行的**所有分片和校验文件**，原样放入应用数据目录的 `voice-engine-packs/`；不要改名、提前解压或混用 V2/V4 分片。之后在“设置 → 扩展与连接 → GPT-SoVITS”选择对应版本并点击安装。

| 版本 | 分片 | 校验文件 | 建议 |
| --- | --- | --- | --- |
| V2 | [`.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.000) · [`.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.001) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.sha256) | **推荐** |
| V4 | [`.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.000) · [`.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.001) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.sha256) | 谨慎试用 |

> **优先使用 V2。** V4 在 Mac 上会占用更多资源，可能造成设备性能下降并让语音合成明显变慢；除非有专门测试需求，否则不建议使用 V4。
