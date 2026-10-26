# CISRead Beta 1 · 1.0.0-beta.1

**CISRead 的内测初始版本。** 从 Beta 1 开始收集使用反馈，后续内测以此为基线迭代。适用 macOS 13+ / Apple Silicon（M 系列 Mac）。

## 本次可以试用

- **论文语境翻译**：分段整理提取的全文，建立可复用语境卡；翻译结合研究主题、定义、专业术语与相关原文。
- **语境卡与术语修正**：查看来源页码、原文依据，为本篇论文保存自定义译法。
- **按论文区分的缓存**：重复选区在相同语境、术语、模型和思考深度下直接复用本机答案；不同论文分别保存。
- **图文解读**：框选图片，结合图注、正文和问题获得中文解释。
- **连续阅读与多标签**：所有页面上下滚动，一个窗口最多同时阅读 8 篇论文。
- **本机恢复与历史**：恢复 PDF、页码、缩放、位置、图文草稿和已完成答案。
- **模型与思考深度选择**：使用本人账号可用模型及其支持的推理档位。
- **CISRead 名称与图标**：白底石墨灰光效图标，尺寸占比已校准；提供中英文 README。

## 下载与安装

下载本 Release 中的 **ZIP 或 DMG，任选一种**，将 `CISRead.app` 放入“应用程序”。更新前正常退出旧版。每个下载文件的 SHA-256 见 `SHA256SUMS`；应用版本、源代码快照和安装包摘要见 `release-manifest.json`。

[安装与使用](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/BETA_GUIDE.md) · [English README](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/README.en.md) · [提交反馈](https://github.com/YouthLiuYS/CISRead-Beta/issues/new?template=bug_report.yml)

## 内测说明

- 本包采用 ad-hoc 完整性签名，**没有 Apple Developer ID 签名及公证**；首次打开可能被 macOS 拦截，请参考安装指南，保留系统安全保护。
- 云端功能使用测试者本人的符合资格的 ChatGPT 套餐。无需额外 API key、本地大模型或单独运行常驻服务；不连接仍可阅读。
- 首次论文语境整理会分段发送提取的全文，后续发送选句及必要语境；图文解读发送主动附加的资料。首次准备和高思考深度会增加用量与等待时间。见[隐私说明](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/PRIVACY.md)。
- 暂无 OCR 文字层和订阅余额读取；模型输出需与原文核对。没有自动更新。
- 仅用于个人非商业学习和试用；包含的运行库遵循其独立非商业许可。安装包不含作者的登录、私人论文、阅读记录或缓存。

## English

**CISRead Beta 1 is the initial CISRead Beta release**, for macOS 13+ on Apple Silicon.

It includes paper-aware Chinese translation, reusable context cards, per-paper terminology corrections and caching, figure interpretation with captions and related text, continuous PDF scrolling, up to eight tabs, local reading restoration and answer history, and model/reasoning-effort controls.

Download either ZIP or DMG and copy `CISRead.app` to Applications. Each tester authorizes their own eligible ChatGPT plan. No separate API key, local model, or independently running service is needed. First-time context preparation sends extracted paper text to OpenAI and consumes plan usage; later requests reuse local context and completed answers where applicable.

This is a personal, noncommercial prerelease with an ad-hoc integrity signature, **not Apple Developer ID signing or notarization**. Consult the installation guide before first launch. The interface and translation output are currently Chinese.
