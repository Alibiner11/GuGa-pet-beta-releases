# GuGa Pet Beta Releases

GuGa Pet 内测安装包、独立能力与引擎安装包发布仓库。

## GPT-SoVITS 音色克隆包

首个发布为 **v0.1.0**，只提供已验真的 macOS Apple Silicon（`darwin-arm64`）版本：

| 包 | 用途 | 推荐 |
| --- | --- | --- |
| GPT-SoVITS V4 | 高质量音色克隆 | 默认推荐 |
| GPT-SoVITS V2 | 少样本克隆兼容档 | 需要旧版兼容时使用 |

每个包由两个 ZIP 分片组成，因为完整引擎包超过 GitHub Release 单文件 2 GiB 限制。咕咕应用会自动下载、拼接、校验、安装并启动；用户不需要安装 Python、Conda 或配置端口。

手动下载时，请下载同一版本的全部 `.zip.000`、`.zip.001` 文件，原样放入咕咕的 `voice-engine-packs` 专属目录，然后在「扩展与连接」中点击对应版本的安装按钮。

每个 Release 同时提供完整 ZIP 的 `.sha256` 校验文件。请在安装前按 Release 页面说明验证下载完整性。
