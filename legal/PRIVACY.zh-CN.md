# Sigla 隐私说明

更新日期：2026 年 7 月 22 日<br>
权利主体：Mr.ZhouPeng

## 数据处理概览

Sigla 是本地 Markdown 阅读、批注和 Agent 反馈交接工具。Sigla 1.0 没有账号系统、广告、行为分析、崩溃遥测和后台云同步。

## 本地保存的数据

以下数据保存在 macOS 应用私有目录：

- 用户登记的文件规范路径、文件名、内容哈希和可用状态。
- 阅读位置、工作区状态、批注、AI 结果缓存和反馈历史。
- 为剪贴板附件生成的私有反馈文件；目录权限为 `0700`，文件权限为 `0600`。
- 界面主题、字号、语言等设置。

API Key 保存在 macOS Keychain。应用数据库只记录随机凭据引用，不保存完整 Key。

## AI 服务

只有用户主动测试连接、生成总结或生成 AI 反馈时，Sigla 才会联系用户选择的 AI 服务商。请求可能包含当前 Markdown 内容、批注、Prompt、模型信息和完成任务所需的上下文。

服务商依据其自身隐私条款处理请求。Sigla 1.0 支持 OpenAI 兼容接口，预设包含 OpenAI 和 DeepSeek。

Sigla 不会使用本地文档训练自己的模型，也不会向 Mr.ZhouPeng 运营的服务器上传文档，因为 Sigla 1.0 没有此类服务器。

## 反馈文件与路径信息

用户主动复制或导出的反馈 Markdown／JSON 可能包含文档名称、内容哈希、批注、AI 建议和源文件绝对路径。该文件离开应用私有目录或被粘贴到 Agent 后，接收方可以读取这些信息，分享前请先检查。

## 删除与保留

- 用户可以在 Sigla 中删除批注、反馈历史、AI 凭据和项目私有数据。
- 卸载应用不会自动删除应用私有数据或 Keychain 条目；手动清理位置见[支持说明](../SUPPORT.md)。
- 导出到用户选择目录的反馈文件由用户自行管理。
- 源 Markdown 通过只读流程处理。Sigla 不提供源 Markdown 的修改、删除、移动、重命名、复制、恢复或格式化操作。

## 系统权限

Sigla 使用用户明确选择或通过 Finder 打开的 Markdown 路径。应用没有通用文件系统、通用 SQL、辅助功能控制、自动化控制或后台录屏权限。Codex 返回功能只激活受支持桌面应用的固定 bundle identifier。

## 联系与变更

不含敏感信息的隐私问题可以通过 [GitHub Issues](https://github.com/z18520736823-coder/sigla-desktop/issues)反馈。疑似安全问题请使用[私密漏洞报告](https://github.com/z18520736823-coder/sigla-desktop/security)。数据处理范围发生变化时，本说明会更新日期并随新版本发布。

[English version](PRIVACY.md)
