# GPT-SoVITS Windows 能力包说明

Windows x64 的 GPT-SoVITS V2 和 V4 是两个独立能力包，分别打包、分别校验、分别安装。它们不属于 GuGu Pet 主应用安装器。

每个版本的发布资产命名如下：

```text
guga-gpt-sovits-v2-win32-x64.zip.000
guga-gpt-sovits-v2-win32-x64.zip.001
guga-gpt-sovits-v2-win32-x64.zip.sha256

guga-gpt-sovits-v4-win32-x64.zip.000
guga-gpt-sovits-v4-win32-x64.zip.001
guga-gpt-sovits-v4-win32-x64.zip.sha256
```

请下载同一版本的全部分片，原样放入 `%APPDATA%\desktop-pet-host\voice-engine-packs\`，不要自行解压、改名或混用 V2/V4 分片。应用会自动合并并验证 `guga-voice-pack.json` 中的引擎、版本和 `win32-x64` 平台字段。

能力包包含已调试的引擎代码、可搬迁运行时和对应模型权重；主应用和 Git 源码仓库均不携带这些大文件。首次安装/启动需要较多磁盘和内存，这是离线运行时与权重的正常开销。
