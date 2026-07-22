<div align="center">
  <img src="docs/assets/sigla-mark.svg" width="112" alt="Sigla logo">
  <h1>Sigla</h1>
  <p><strong>The human review layer for AI-generated Markdown.</strong></p>
  <p>Turn long, dense Agent output into evidence-linked insights, source-anchored annotations, and actionable feedback—while your original files stay read-only.</p>
  <p>
    <a href="https://z18520736823-coder.github.io/sigla-desktop/"><strong>Product page</strong></a>
    ·
    <a href="https://github.com/z18520736823-coder/sigla-desktop/releases/tag/v1.0.0-preview.1"><strong>Download for macOS</strong></a>
    ·
    <a href="README.zh-CN.md">简体中文</a>
  </p>
</div>

> **Public Preview · macOS 11+ · Apple Silicon and Intel**<br>
> Free to use during the preview. Source code remains private.

AI writes more Markdown than anyone has time to read. Sigla gives that output a reviewable shape: one central conclusion, the few ideas that matter, precise annotations anchored to the source, and a structured brief that can go straight back to Codex or another Agent.

## The review problem

- **Too long to read. What actually matters?**
- **When feedback matters, can it point to the exact source?**
- **When one idea changes, are the related tasks, constraints, and acceptance criteria still clear?**
- **No API. No connection. Can the review continue?**

## Four principles, one review layer

### 1. AI-powered Clarity

**Powered by OpenAI or DeepSeek, Sigla turns long Markdown documents into one central conclusion and 3–5 key takeaways. Every insight is linked back to its source.**

Use your own API key. Sigla stores it in macOS Keychain and sends document content to the provider only when you explicitly run an AI action.

### 2. Effortless Annotation

**Draw a box around any passage and add a comment, question, or change request. Every annotation stays attached to its exact source—without touching the original Markdown.**

Annotations live in Sigla's private local database. When the document changes externally, Sigla rechecks the anchor and asks for confirmation when the match is uncertain.

### 3. Agent-ready Feedback

**Sigla turns selected annotations into a clear editing brief with exact locations, requested changes, and acceptance criteria—ready to send back to Codex or another Agent. Related or conflicting requests remain explicit.**

Your original wording and source evidence remain part of the handoff, so the next Agent receives the context needed to make a precise change.

### 4. Offline Continuity

**No API or internet connection is required for reading, rendering, annotation, and local feedback. AI runs only when you choose to use it, while your original files remain read-only.**

Sigla has no source-file operation for editing, deleting, moving, renaming, or restoring Markdown. Reading state, annotations, AI cache, and feedback history stay in the app's private local storage.

## See Sigla in action

<!-- SCREENSHOT SLOT 01: docs/assets/screenshots/01-hero-light.png — light three-pane interface with AI summary -->
<!-- SCREENSHOT SLOT 02: docs/assets/screenshots/02-dark-bilingual-reading.png — dark mode with Chinese/English typography, code, table, and Mermaid -->
<!-- SCREENSHOT SLOT 03: docs/assets/screenshots/03-ai-evidence-anchors.png — AI summary linked to source anchors -->
<!-- SCREENSHOT SLOT 04: docs/assets/screenshots/04-annotation-feedback-handoff.png — box annotations converted to Agent-ready feedback -->
<!-- SCREENSHOT SLOT 05: docs/assets/screenshots/05-codex-default-app-flow.png — Codex and default Markdown opener workflow -->

> Product screenshots are being prepared for the public launch. The private staging repository intentionally keeps these five positions reserved.

## From Agent output to human decision

```text
Agent creates → Sigla distills → You review → AI structures feedback → Agent revises → Sigla verifies
```

1. Open a Markdown file from Finder, Codex, or inside Sigla.
2. Read with bilingual typography, light/dark themes, GFM, code blocks, tables, and Mermaid.
3. Ask OpenAI or DeepSeek for a source-linked reading map when you need it.
4. Draw boxes around exact passages and record comments, questions, or change requests.
5. Turn selected annotations into an actionable feedback bundle.
6. Return the bundle to Codex or another Agent, then inspect the external revision in Sigla.

## Capability proof

| Area | What Sigla provides |
| --- | --- |
| Reading | Safe GitHub Flavored Markdown, bilingual typography, code, tables, Mermaid, collapsible sections |
| Review | Box annotations, comments, questions, change requests, exact source anchors, re-anchoring |
| AI | OpenAI and DeepSeek BYOK, streaming results, source evidence, cancellation, cache, local fallback |
| Agent workflow | Structured feedback bundles, Codex return flow, feedback history, external-change verification |
| macOS | Finder integration, optional default Markdown opener, menu-bar presence, system/light/dark themes |
| Privacy | No account, ads, analytics, crash telemetry, or background cloud sync |

## Download and install

Download **Sigla 1.0.0 Public Preview** from [GitHub Releases](https://github.com/z18520736823-coder/sigla-desktop/releases/tag/v1.0.0-preview.1).

- Universal 2: Apple Silicon and Intel
- Minimum system: macOS 11.0
- Distribution: DMG
- Signature: ad-hoc with hardened runtime
- Apple notarization: not yet completed
- Updates: manual download

After opening the DMG, drag Sigla into **Applications**. For the first launch, open **Finder → Applications**, Control-click Sigla, and choose **Open**. If macOS still blocks the app, allow it in **System Settings → Privacy & Security**.

Verify the download:

```text
SHA-256: eb47705320e80943b916e430e4dd3cc3b370c0caf56a8b53cbd132c0cd961ecc
```

Detailed steps are available in [Support](SUPPORT.md).

## Privacy and AI boundaries

- Source Markdown is opened through a strict read-only workflow.
- API keys are stored in macOS Keychain, never in the Sigla database.
- Document content reaches OpenAI or DeepSeek only after an explicit AI action.
- Sigla has no account system, telemetry service, or document-sync server.
- Exported feedback can contain document names, paths, quotes, annotations, and AI suggestions. Review it before sharing.

Read the complete [Privacy Notice](legal/PRIVACY.md), [EULA](legal/EULA.md), and [Security Policy](SECURITY.md).

## FAQ

### Is Sigla open source?

No. This repository contains public product documentation, community resources, and release downloads. The Sigla source code remains private under a proprietary license.

### Does Sigla edit my Markdown files?

Sigla does not expose operations to edit, delete, move, rename, or restore source Markdown. Annotations and review state are stored separately in the app's private local database.

### Can I use Sigla without AI?

Yes. Reading, Markdown rendering, annotation, file monitoring, and local basic feedback continue without an API key or network connection.

### Which AI providers are supported?

Sigla 1.0 includes presets for OpenAI and DeepSeek through a bring-your-own-key workflow. AI is optional and initiated by the user.

### Does Sigla upload my documents?

Sigla has no document-sync server. When you explicitly request an AI summary or AI-organized feedback, the necessary document content and review context are sent directly to the provider you selected.

## Community

- [Report a bug](https://github.com/z18520736823-coder/sigla-desktop/issues/new?template=bug.yml)
- [Request a feature](https://github.com/z18520736823-coder/sigla-desktop/issues/new?template=feature.yml)
- [Share experience feedback](https://github.com/z18520736823-coder/sigla-desktop/issues/new?template=experience.yml)
- [Join Discussions](https://github.com/z18520736823-coder/sigla-desktop/discussions)

If Sigla makes Agent output easier to understand and review, a GitHub Star helps more people discover it.

## License

Copyright © 2026 Mr.ZhouPeng. All rights reserved. Sigla is proprietary software. See [LICENSE](LICENSE) and the [End User License Agreement](legal/EULA.md).
