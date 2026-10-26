# CISRead

简体中文 · [English](README.en.md)

<img src="icon.png" alt="CISRead 图标" width="88" />

**CISRead**（原名 PaperRead）是 **CISArch** 团队面向英文论文阅读的 macOS 桌面工具，正在个人非商业内测。**CIS** 是团队共同品牌标识，另一款在研产品为 **CISCube**。

软件已更名为 CISRead。为兼容现有下载与反馈链接，仓库地址保留 `PaperRead-Beta`。

**当前公开下载：PaperRead Beta 0.8.0-beta.1** · **macOS 13+ / Apple Silicon（M 系列芯片）**

[下载安装包](https://github.com/YouthLiuYS/PaperRead-Beta/releases/tag/v0.8.0-beta.1) · [安装与使用](BETA_GUIDE.md) · [反馈问题](https://github.com/YouthLiuYS/PaperRead-Beta/issues/new?template=bug_report.yml) · [隐私说明](PRIVACY.md)

> 本机研发版本为 CISRead 0.9.1-beta.1，已包含论文语境卡与术语修正；这些功能尚未包含在当前公开的 0.8.0 安装包中。新名称安装说明见 [CISRead 指南](CISREAD_BETA_GUIDE.md)，新包以未来 Release 为准。

## 当前公开安装包可以做什么

- 打开 PDF 后连续上下滚动；一个窗口最多同时保留 8 篇论文标签。
- 鼠标划选英文句子，在右侧查看中文译文，继续在原文中阅读。
- 框选论文图，添加图注、相关正文和问题，获得中文图文解释。
- 选择模型和支持的思考深度；重复内容自动复用缓存，减少重复请求。
- 本机保存阅读位置、图文草稿和答案历史，退出后恢复。

## 参加内测

1. 使用符合系统要求的 Mac，下载本页 Releases 中的 ZIP 或 DMG。
2. 安装后点击 **Continue with ChatGPT**，在系统浏览器中登录你自己的账号并授权套餐使用。云端功能需要符合资格的 ChatGPT Plus / Pro 账号；实际可用性、模型和额度由 OpenAI 决定。不连接也可阅读 PDF。
3. 打开一篇有文字层的英文论文，划选句子试用翻译。图文资料仅在点击解读时发送。
4. 用应用内“反馈问题”入口报告遇到的问题，尽量附复现步骤和不含隐私的截图。

内测免费，推理使用测试者本人的套餐；软件不提供共享账号、额度或 API key。无需另外安装 Node、本地大模型或启动常驻服务。没有自动更新，后续版本请从 Releases 手动下载。

## 当前限制

- 只发布 Apple Silicon macOS 版本，Windows、Linux 和 Intel Mac 暂未验证。
- 当前包使用 ad-hoc 完整性签名，**没有 Apple Developer ID 签名和公证**；首次打开可能被系统拦截，请先阅读[安装说明](BETA_GUIDE.md)。这不是 App Store 发布。
- 扫描 PDF 暂无 OCR 文字层；可框选图片进行图文解读。
- 套餐余额无法在软件中实时读取，面板中的缓存统计不是余额。
- 模型解释可能出错，尤其是公式、数值和图表结论，请与论文原文核对。

本阶段用于个人学习、研究和非商业体验。所包含的 Sign in with ChatGPT DevKit 及修改受[独立非商业许可](licenses/SIWC-LICENSE.txt)约束，商业用途不在本次发布范围内。CISRead 是 CISArch 的独立项目，并非 OpenAI 或 Anthropic 的官方产品。

此仓库用于内测包分发、使用说明和反馈；不包含原私有开发仓库的历史、作者的账号凭据或论文资料。

![公开版 PaperRead Beta 0.8.0 首次使用界面：内置演示与未连接状态](preview.png)

套餐接入范围参考 [OpenAI 官方本地工具说明](https://developers.openai.com/cookbook/articles/sign-in-with-chatgpt)。
