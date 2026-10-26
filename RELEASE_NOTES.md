# PaperRead Beta · 0.8.0-beta.1

PaperRead 首个个人非商业内测版本。支持 macOS 13+、Apple Silicon / M 系列 Mac。

## 本次可以试用

- 整篇 PDF 连续滚动，划选英文句子显示中文译文。
- 框选论文图，结合图注和相关正文进行中文解读。
- 选择账号可用模型与支持的思考深度。
- 单窗口多标签、阅读位置恢复、图文草稿和答案历史。
- 持久翻译缓存、跨标签复用及本机调用统计。
- 跟随系统深浅色界面与石墨灰材质图标。

## 下载与使用

只需下载 ZIP 或 DMG 中的一种。ZIP 解压或打开 DMG 后，将 `PaperRead.app` 拖入“应用程序”。更新前退出旧版，已有资料会保留。SHA256SUMS 可用于核对下载文件。

云端功能使用测试者**本人的**符合资格的 ChatGPT Plus / Pro 套餐，需要自行在系统浏览器授权；无需额外 API key、本地大模型或常驻服务。不登录也可阅读 PDF。

## 内测须知

- 此包采用 ad-hoc 完整性签名，**没有 Apple Developer ID 签名及公证**。首次启动可能被系统拦截；请先阅读[安装说明](https://github.com/YouthLiuYS/PaperRead-Beta/blob/main/BETA_GUIDE.md)。不关闭系统安全保护。
- 暂不支持 Windows、Linux 或已验证的 Intel Mac 版本。扫描 PDF 暂无 OCR，套餐余额暂无法直接读取。
- 没有自动更新；后续版本从本仓库 Releases 手动下载。
- 仅用于个人非商业学习和试用；所含 SIWC 运行库遵循独立非商业许可。
- 论文在本机解析，仅选文或主动附加的图文资料发送给 OpenAI。安装包不含作者登录或论文记录。
- 这是独立内测项目，并非 OpenAI 或 Anthropic 的官方产品。

[使用说明](https://github.com/YouthLiuYS/PaperRead-Beta#readme) · [反馈问题](https://github.com/YouthLiuYS/PaperRead-Beta/issues/new?template=bug_report.yml) · [隐私说明](https://github.com/YouthLiuYS/PaperRead-Beta/blob/main/PRIVACY.md)
