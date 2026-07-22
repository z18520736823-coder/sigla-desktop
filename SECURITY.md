# Security Policy · 安全政策

## Supported version

Security fixes currently target the latest Sigla Public Preview release.

## Report a vulnerability

Please use GitHub's **Private vulnerability reporting** for security issues. Do not open a public Issue for a suspected vulnerability.

Include the affected version, macOS version, reproduction steps, expected impact, and the smallest safe proof of concept. Remove API keys, private paths, personal documents, and credentials before submitting.

We will acknowledge a report through GitHub, investigate it, and publish a coordinated fix or mitigation when confirmed. A response-time guarantee is not yet available during the Public Preview.

## Product security boundaries

- Source Markdown is handled through a read-only workflow.
- Sigla exposes no source-file operation for editing, deleting, moving, renaming, copying, restoring, or formatting Markdown.
- Application state is stored in a private local SQLite database.
- API keys are stored in macOS Keychain.
- AI requests originate from the Rust backend and run only after an explicit user action.
- The WebView has no general filesystem, SQL, Keychain, shell, or arbitrary HTTP capability.
- Feedback exports are created as new files and reject existing targets, symbolic links, hard links, and directory-identity changes.

These controls protect actions performed by Sigla. They cannot prevent changes made by the operating system, another application, storage failure, or a user-directed export.

---

## 支持版本

安全修复当前面向最新的 Sigla 公开预览版。

## 报告安全问题

请使用 GitHub 的 **Private vulnerability reporting** 提交安全问题。疑似漏洞请勿公开创建 Issue。

报告中请包含受影响版本、macOS 版本、复现步骤、预期影响和最小安全验证样例。提交前请移除 API Key、私人路径、个人文档和凭据。

我们会通过 GitHub 确认报告、开展调查，并在问题确认后协调发布修复或缓解方案。公开预览期间暂不承诺固定响应时间。

## 产品安全边界

- 源 Markdown 通过只读流程处理。
- Sigla 不提供源 Markdown 的修改、删除、移动、重命名、复制、恢复或格式化操作。
- 应用状态保存在本地私有 SQLite 数据库。
- API Key 保存在 macOS Keychain。
- AI 请求由 Rust 后端发起，并且只在用户主动操作后运行。
- WebView 没有通用文件系统、SQL、Keychain、Shell 或任意 HTTP 权限。
- 反馈导出采用新文件创建机制，并拒绝已有目标、符号链接、硬链接和目录身份变化。

这些控制约束 Sigla 自身执行的操作。操作系统、其他应用、存储故障或用户主动导出带来的变化不在其控制范围内。
