# GPT-SoVITS 音色克隆包 v0.1.0（macOS Apple Silicon）

面向 GuGu Pet 内测的首个本地音色克隆引擎发布。

## 内容

- GPT-SoVITS V2：macOS 内测推荐的音色克隆包。
- GPT-SoVITS V4：可选试用的高质量音色克隆包；在 macOS 上不作为默认推荐。
- 内置已调试的可搬迁 Python 运行时、引擎代码、中文前端模型与对应版本权重。
- 仅支持 macOS Apple Silicon（`darwin-arm64`，M 系列芯片）。

## 直接下载

每个版本必须下载同一版本的两个分片及其校验文件；不要改名、单独解压或混用 V2/V4。

| 版本 | 分片 | 校验文件 |
| --- | --- | --- |
| V2（推荐） | [`.zip.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.000) · [`.zip.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.001) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v2-darwin-arm64.zip.sha256) |
| V4（谨慎试用） | [`.zip.000`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.000) · [`.zip.001`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.001) | [`.sha256`](https://github.com/Alibiner11/GuGu-pet-beta-releases/releases/download/v0.1.0/guga-gpt-sovits-v4-darwin-arm64.zip.sha256) |

> **macOS 用户请优先安装 V2。** V4 在 Mac 设备上会使用更多系统资源，可能导致设备性能下降，并使语音合成速度明显变慢。除非需要专门验证 V4，否则不推荐在 macOS 内测环境中使用。

## 使用方式

在 GuGu Pet 的「设置 → 扩展与连接」选择 GPT-SoVITS V2（推荐）或 V4，点击安装即可。应用会自动下载、合并分片、校验平台、安装、接入并启动本地服务。

如需手动下载，请下载同一版本的 `.zip.000` 与 `.zip.001` 两个分片，原样放到应用数据目录内的 `voice-engine-packs/`，随后在应用内点击安装。不要自行解压、改名或调整目录结构。

## 完整性校验

每个版本都附有完整 ZIP 的 `.sha256` 文件。把分片拼接为原 ZIP 后，应与该校验值一致；应用安装时也会校验引擎、版本与系统平台。

## 已知范围

- 当前只发布 V2 与 V4；其他音色克隆引擎暂不在内测渠道提供。
- 首次安装和首次启动需要较长时间，并占用较多本地磁盘与内存，这是完整离线运行时与模型权重的正常开销。
