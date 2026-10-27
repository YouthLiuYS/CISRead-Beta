# CISRead Beta 2 · 1.0.0-beta.2

本次修复译文和图文解释中直接显示 LaTeX 与 Markdown 源码的问题，让公式和正文可以一起阅读。适用 macOS 13+ / Apple Silicon（M 系列 Mac）。Beta 1 保持为 CISRead 内测初始版本。

## 本次更新

- **公式正常显示**：支持行内与独立公式，以及分式、根号、上下标、求和、矩阵。兼容 `\(...\)`、`\[...\]`、`$...$`、`$$...$$`。
- **正文排版**：粗体、标题、列表、表格和代码正常显示；超宽公式在自身区域横向滚动，不撑开窗口。
- **已有答案立即受益**：本机缓存和答案历史直接重新排版，无需再次调用模型，不消耗额外套餐用量。原始答案、论文语境、术语修正及缓存键保持兼容。
- **流式与异常处理**：未输出完整的公式先保留为文字，闭合后排版；无法识别的公式保留源文，其他内容继续显示。
- **本机渲染**：公式字体随应用打包，不加载外部图片或渲染服务；跟随系统深浅色。复制答案继续保留原始 Markdown / LaTeX。

现有 ChatGPT 套餐接入、模型选择和思考深度选择继续保留。更新只需退出应用并替换安装包，登录、论文、阅读位置、语境、历史和缓存无需重置。

## 下载与安装

下载本 Release 中的 **ZIP 或 DMG，任选一种**，将 `CISRead.app` 放入“应用程序”。更新前正常退出旧版。每个下载文件的 SHA-256 见 `SHA256SUMS`；应用版本、源代码快照和安装包摘要见 `release-manifest.json`。

[安装与使用](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/BETA_GUIDE.md) · [English README](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/README.en.md) · [提交反馈](https://github.com/YouthLiuYS/CISRead-Beta/issues/new?template=bug_report.yml)

## 内测说明

- 本包采用 ad-hoc 完整性签名，**没有 Apple Developer ID 签名及公证**；首次打开方式见安装指南。
- 云端功能使用测试者本人符合资格的 ChatGPT 套餐。无需额外 API key、本地大模型或单独运行常驻服务；不连接仍可阅读。
- 首次论文语境整理会分段发送提取的全文，后续发送选句及必要语境；图文解读发送主动附加的资料。见[隐私说明](https://github.com/YouthLiuYS/CISRead-Beta/blob/main/PRIVACY.md)。
- 暂无 OCR 文字层和订阅余额读取；公式排版不会修正模型理解或原文提取错误，请核对原文。没有自动更新。
- 仅用于个人非商业学习和试用；包含的运行库遵循其独立非商业许可。安装包不含作者的登录、私人论文、阅读记录或缓存。

## English

**CISRead Beta 2** fixes raw LaTeX and Markdown appearing in translation and figure answers. Inline and display equations, fractions, roots, subscripts, sums, matrices, emphasis, lists, and tables now render as formatted content. Long equations scroll locally.

Existing cached and historical answers are formatted on the device without another inference. Formula fonts are bundled, incomplete streamed equations remain text until closed, and copying preserves the original Markdown / LaTeX. Existing plan authorization, model and reasoning-effort controls, paper context, terminology, reading records, and caches are retained.

Download either ZIP or DMG and copy `CISRead.app` to Applications after quitting the previous version. For macOS 13+ on Apple Silicon. Beta 1 remains the initial CISRead Beta release. This personal, noncommercial prerelease uses an ad-hoc integrity signature, not Apple Developer ID signing or notarization. The interface and translation output are currently Chinese.
