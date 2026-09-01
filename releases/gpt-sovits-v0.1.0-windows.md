# GPT-SoVITS Windows 能力包说明

Windows x64 的 GPT-SoVITS V2 和 V4 将以独立能力包形式发布，不属于 GuGu Pet 主应用安装器。

## 当前状态

当前公开 Release **尚未提供 Windows 专用的 GPT-SoVITS 能力包**。请勿下载、导入或混用 macOS 的 `darwin-arm64` 分片；它们只适用于 M 系列芯片 Mac，不能在 Windows 上安装。

待 Windows 专用资产发布后，会在对应引擎 Release 中提供 V2/V4 的分片、校验文件和直达链接。届时请下载同一版本的全部分片，原样放入 `%APPDATA%\desktop-pet-host\voice-engine-packs\`，不要自行解压、改名或混用 V2/V4 分片。应用会自动合并并验证 `guga-voice-pack.json` 中的引擎、版本和 `win32-x64` 平台字段。

能力包会包含已调试的引擎代码、可搬迁运行时和对应模型权重；主应用和 Git 源码仓库均不携带这些大文件。首次安装/启动需要较多磁盘和内存，这是离线运行时与权重的正常开销。
