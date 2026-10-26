# CISRead

[简体中文](README.md) · English

<img src="icon.png" alt="CISRead icon" width="88" />

**CISRead**, formerly **PaperRead**, is a macOS reader for English research papers from the **CISArch** team. The **CIS** prefix identifies the team's products, including **CISCube**, another product under development.

The repository URL remains `PaperRead-Beta` so existing download and feedback links continue to work.

## Download status

**Current public installer: PaperRead Beta `0.8.0-beta.1`**, for **macOS 13+ on Apple Silicon**.

[Download ZIP or DMG](https://github.com/YouthLiuYS/PaperRead-Beta/releases/tag/v0.8.0-beta.1) · [Report an issue](https://github.com/YouthLiuYS/PaperRead-Beta/issues/new?template=bug_report.yml) · [Privacy for the public 0.8 build](PRIVACY.md)

The current development build is named **CISRead `0.9.1-beta.1`**. It adds paper-context cards and per-paper terminology corrections. These newer features and the new application name are **not included in the current public 0.8 installer**. A new CISRead installer will be identified by its own future Release; existing files are not replaced silently.

## What the public Beta can do

- Read a PDF by scrolling continuously through its pages.
- Select English text and view a Chinese translation beside the original.
- Capture a figure, attach its caption and related text, and ask for a Chinese explanation.
- Choose an available model and its supported reasoning effort.
- Reuse cached answers to avoid exact duplicate requests.
- Keep up to eight papers in tabs in one window, with local positions, drafts, and answer history.

The app currently uses Chinese interface labels and translates into Chinese. English documentation does not imply an English interface or English output.

## Install the current public download

1. Download either the ZIP or the DMG; you only need one format.
2. Extract the ZIP or open the DMG, then copy **`PaperRead.app`** to **Applications**. The public 0.8 download still uses this original name. Quit an existing instance before replacing it.
3. Launch the app and choose **Continue with ChatGPT**. Sign in to your own eligible account in the system browser and authorize plan usage. Model access and limits depend on OpenAI and your account.
4. Open an English PDF with a text layer and select a sentence. For a figure, select the figure mode, capture the relevant area, add supporting text, and explicitly start interpretation.

The packaged app needs no separate API key, local language model, Node installation, or independently running server. Reading a PDF remains available when the plan is disconnected. There is no automatic updater.

## Signature and checksums

The public Beta has an ad-hoc integrity signature. It is **not Developer ID signed or Apple notarized**, and macOS may block its first launch. Verify that the file came from this repository's Release and compare its SHA-256 with `SHA256SUMS` if needed.

If you trust the source, follow [Apple's instructions for opening an unnotarized app](https://support.apple.com/102445), including the app-specific decision in Privacy & Security. Do not disable Gatekeeper or system protection. Stop if macOS reports malicious content. Managed devices may not permit an exception.

## Plan usage and privacy

Every tester authorizes their own eligible ChatGPT plan. The Beta does not distribute a developer account, credentials, or shared quota. It manages its own authorization rather than reading your Codex login files. Eligibility, models, and available usage are determined by OpenAI; see the [official local-tool documentation](https://developers.openai.com/cookbook/articles/sign-in-with-chatgpt).

For **the public 0.8 build**, PDFs are parsed locally and the selected text or explicitly supplied figure evidence is sent for inference. **The newer CISRead development build** additionally sends extracted paper text when first building a paper-context card, then sends selections with the required context. The [CISRead privacy document](CISREAD_PRIVACY.md) describes that newer behavior.

Local request and cache statistics are not a real-time subscription balance. The app links to the official usage page. Higher reasoning effort may take longer and consume more plan usage.

The application has no automatic telemetry, crash upload, or feedback submission. Reading data, caches, and authorization have separate local controls. Public issue reports should not contain private papers, login files, passwords, or sensitive screenshots.

## Limitations and feedback

Only the Apple Silicon macOS build has been validated. Windows, Linux, and Intel Mac builds are not provided here. There is no OCR text layer for scanned PDFs; selected images can be discussed through figure interpretation. Model output can be wrong, especially for equations, measurements, and chart conclusions, so check the original evidence.

Use [GitHub Issues](https://github.com/YouthLiuYS/PaperRead-Beta/issues/new?template=bug_report.yml) and include the app version, macOS version and chip, reproduction steps, expected behavior, and actual behavior. Share only material you are allowed to publish.

This is a free, personal, noncommercial Beta. The included Sign in with ChatGPT runtime is governed by its own [noncommercial license](licenses/SIWC-LICENSE.txt). CISRead is an independent CISArch project, not an official OpenAI or Anthropic product. This distribution repository contains installers, documentation, and feedback templates; it does not publish the private source repository or its history.

![Public PaperRead Beta 0.8 interface, showing the original demo and disconnected state](preview.png)

[New CISRead installation and compatibility guide](CISREAD_BETA_GUIDE.md) · [中文说明](README.md)
