# CISRead Beta 4 · 1.0.0-beta.4

加入应用内下载、签名校验与重启安装，不用手动替换应用。适用 macOS 13+ / Apple Silicon（M 系列 Mac）。Beta 1 保持为 CISRead 内测初始版本。

## 本次更新

- **应用内下载**：通过右上角 **⋯ → 检查更新…** 或 macOS **CISRead / 帮助** 菜单查看新版本和发布说明，点击 **下载更新**，直接查看下载进度。
- **继续阅读**：下载期间可关闭弹窗、继续阅读或取消下载；安装包准备好后可稍后再安装。
- **重启并安装**：签名校验通过后点击 **重启并安装**，自动完成安装并重新打开 CISRead。
- **保留资料**：重启前保存全部论文标签、阅读位置、缩放、答案历史与图文草稿，沿用原来的登录、语境、术语、缓存及模型/思考深度设置。
- **失败保护**：资料保存失败会暂停重启；更新清单或安装包签名校验失败会阻止安装，保留当前应用与本机资料。网络失败可重新下载。
- **按需更新**：主动检查和下载，不调用翻译模型，不发送论文或套餐凭据，没有独立常驻更新服务。

继续保留论文语境翻译、图文解读、多标签连续阅读和公式排版。已有缓存和答案历史无需重新调用模型。

## 安装与升级

**首次安装，或从 Beta 1–3 升级到 Beta 4**：下载名称以 `CISRead-Beta-` 开头的 ZIP / DMG，任选一种；正常退出旧版，将 `CISRead.app` 放入“应用程序”并替换，再启动。此后新版可以直接在 CISRead 内下载和重启安装。

`CISRead-Update-…zip` 与 `appcast.xml` 供应用内更新组件使用，首次安装请选择普通 Beta 安装包。校验和见 `SHA256SUMS`，版本与构建信息见 `release-manifest.json`。

[安装与使用](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/BETA_GUIDE.md) · [English README](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/README.en.md) · [提交反馈](https://github.com/YouthLiuYS/CISRead-Beta/issues/new?template=bug_report.yml)

## 内测说明

- 应用使用 ad-hoc 完整性签名，没有 Apple Developer ID 签名及公证。首次打开方式见安装指南；系统可能要求本人授权安装更新。
- 更新组件 Sparkle 校验独立的 Ed25519 更新签名。更新仅替换应用程序包，用户资料目录保持原位。
- 每名测试者授权本人符合资格的 ChatGPT 套餐。无需额外 API key、本地大模型或独立常驻服务。不登录仍可阅读和更新。
- 数据行为见[隐私说明](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/PRIVACY.md)。更新不消耗翻译套餐用量。
- 暂无 OCR 文字层和订阅余额读取。模型及公式内容需与原文核对。
- 仅用于个人非商业学习与试用；包含的运行库遵循其独立许可。安装包不含作者登录、私人论文、阅读记录或缓存。

## English

CISRead Beta 4 adds **in-app download, signature verification, and restart-to-install updates**. Check for a new release from the app menu or macOS application/Help menus, download with progress, and choose **重启并安装** once the verified update is ready. You can continue reading, dismiss the dialog, or cancel during download.

Before restart, CISRead saves all paper tabs, reading positions, zoom levels, history, and figure drafts. Existing authorization, paper context, terminology, translation cache, and model/reasoning preferences remain in place. A failed save stops restart; invalid feed or archive signatures block installation. Sparkle verifies updates using a pinned Ed25519 key. Updates replace only the application bundle.

Checks and downloads are manual public requests without paper contents or plan credentials; they do not use translation inference. No independently running update service is required. macOS may request installation authorization when needed.

**Beta 1–3 users must install Beta 4 once using a regular `CISRead-Beta-` ZIP or DMG.** Later releases can be installed inside CISRead. The `CISRead-Update-` ZIP and `appcast.xml` are updater artifacts. For macOS 13+ on Apple Silicon; personal noncommercial prerelease, ad-hoc signed without Apple Developer ID signing or notarization. The interface and translation output are currently Chinese.
