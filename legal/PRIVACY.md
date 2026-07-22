# Sigla Privacy Notice

Updated: July 22, 2026<br>
Rights holder: Mr.ZhouPeng

## Overview

Sigla is a local Markdown reading, annotation, and Agent-feedback application. Sigla 1.0 has no account system, advertisements, behavioral analytics, crash telemetry, or background cloud sync.

## Data stored locally

Sigla stores the following data in the macOS private application directory:

- Registered canonical paths, file names, content hashes, and availability state.
- Reading position, workspace state, annotations, AI result cache, and feedback history.
- Private feedback files generated for clipboard attachments; their directory uses `0700` permissions and files use `0600` permissions.
- Theme, font size, language, and other preferences.

API keys are stored in macOS Keychain. The Sigla database stores only a random credential reference and does not store the complete key.

## AI services

Sigla contacts the selected AI provider only when you explicitly test a connection, generate a summary, or generate AI-organized feedback. A request may contain the current Markdown content, annotations, prompt, model information, and the context required to complete the task.

The provider processes the request under its own privacy terms. Sigla 1.0 supports an OpenAI-compatible interface with presets for OpenAI and DeepSeek.

Sigla does not use local documents to train a model of its own and does not upload documents to a server operated by Mr.ZhouPeng, because Sigla 1.0 has no such server.

## Feedback files and path information

Feedback Markdown or JSON that you explicitly copy or export may contain the document name, content hash, annotations, AI suggestions, and absolute source path. After the file leaves Sigla's private directory or is pasted into an Agent, the recipient can read that information. Review it before sharing.

## Deletion and retention

- You can delete annotations, feedback history, AI credentials, and project-private state within Sigla.
- Uninstalling the application does not automatically remove private application data or Keychain entries. See [Support](../SUPPORT.md) for manual cleanup locations.
- You manage feedback files exported to a chosen directory.
- Source Markdown is handled through a read-only workflow. Sigla exposes no source operation for editing, deleting, moving, renaming, copying, restoring, or formatting Markdown.

## System permissions

Sigla uses Markdown paths you explicitly select or open through Finder. It has no general filesystem, general SQL, accessibility-control, automation-control, or background screen-recording permission. The Codex return action activates only the fixed bundle identifier of the supported desktop application.

## Contact and changes

Use [GitHub Issues](https://github.com/z18520736823-coder/sigla-desktop/issues) for privacy questions that contain no sensitive data. Use [private vulnerability reporting](https://github.com/z18520736823-coder/sigla-desktop/security) for a suspected security issue. This notice will be updated when the data-handling scope changes.

[简体中文版本](PRIVACY.zh-CN.md)
