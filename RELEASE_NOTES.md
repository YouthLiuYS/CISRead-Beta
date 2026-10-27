# CISRead Beta 3 · 1.0.0-beta.3

加入应用内“检查更新”，方便查看新版本、阅读更新内容和下载兼容的安装包。适用 macOS 13+ / Apple Silicon（M 系列 Mac）。Beta 1 保持为 CISRead 内测初始版本。

## 本次更新

- **应用内检查更新**：入口位于右上角 **⋯ → 检查更新…**，以及 macOS 的 **CISRead / 帮助** 菜单。
- **清楚的检查结果**：区分有新版本、已是最新、本机版本领先、暂无公开版本，以及网络错误；Beta 序号按版本规则比较，避免误判或降级。
- **更新内容与下载**：在应用内阅读发布说明；有适用于当前设备的新安装包时，点击“下载更新”在系统浏览器下载。
- **保留阅读状态**：下载后正常退出，将新应用拖入“应用程序”并替换。已有登录、论文、位置、语境、缓存、历史和思考深度设置保留。
- **按需检查**：不需要登录即可检查，不调用翻译模型，不发送论文或套餐凭据。网络失败、超时或发布服务限流时可以重试；点击外部或按 Esc 关闭窗口。

继续包含 Beta 2 的公式排版：译文、图文解释和历史支持分式、根号、上下标、求和与矩阵，兼容常见 LaTeX 分隔符；旧缓存直接获得排版，无需重新调用模型。现有套餐接入、论文语境和模型/思考深度选择继续保留。

## 下载与安装

本 Release 中的 **ZIP 或 DMG 任选一种**，退出旧版后将 `CISRead.app` 放入“应用程序”并替换。文件校验和见 `SHA256SUMS`，版本和源代码快照见 `release-manifest.json`。应用内检查仅识别已经公开发布的版本。

[安装与使用](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/BETA_GUIDE.md) · [English README](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/README.en.md) · [提交反馈](https://github.com/YouthLiuYS/CISRead-Beta/issues/new?template=bug_report.yml)

## 内测说明

- 使用 ad-hoc 完整性签名，没有 Apple Developer ID 签名及公证。首次打开方式见安装指南。更新下载后按提示手动替换应用。
- 每名测试者授权本人符合资格的 ChatGPT 套餐。无需额外 API key、本地大模型或独立常驻服务。不登录仍可阅读和检查更新。
- 论文语境与图文功能的数据行为见[隐私说明](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/PRIVACY.md)。检查更新不消耗翻译套餐用量。
- 暂无 OCR 文字层和订阅余额读取。模型及公式内容需与原文核对。
- 仅用于个人非商业学习与试用；包含的运行库遵循其独立非商业许可。安装包不含作者登录、私人论文、阅读记录或缓存。

## English

CISRead Beta 3 adds **Check for Updates** to the in-app menu and macOS application/Help menus. The dialog compares published versions, includes Betas on the Beta channel, displays release notes, and offers a compatible installer when available. Numeric Beta ordering and stable-release precedence prevent incorrect downgrade suggestions. Errors and timeouts are shown explicitly and can be retried.

Checks are manual, anonymous GitHub release queries. They do not send papers or plan credentials and do not use translation inference. Downloads open in your system browser; quit CISRead and replace it in Applications. Existing authorization, reading data, caches, and model/reasoning settings remain in place. Escape or a click outside closes the dialog.

This version retains Beta 2's local math/Markdown rendering for current answers, caches, and history. Beta 1 remains the initial CISRead Beta release. For macOS 13+ on Apple Silicon; personal noncommercial prerelease with an ad-hoc integrity signature, without Apple Developer ID signing or notarization. The interface and translation output are currently Chinese.
