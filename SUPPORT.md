# Sigla Support · 支持与安装

[English](#english) · [简体中文](#简体中文)

## English

### Install

1. Download `Sigla_1.0.0_universal.dmg` from the [Public Preview release](https://github.com/z18520736823-coder/sigla-desktop/releases/tag/v1.0.0-preview.1).
2. Confirm the SHA-256 value is `eb47705320e80943b916e430e4dd3cc3b370c0caf56a8b53cbd132c0cd961ecc`.
3. Open the DMG and drag Sigla into **Applications**.
4. For the first launch, open **Finder → Applications**, Control-click Sigla, and choose **Open**.
5. If macOS still blocks the app, open **System Settings → Privacy & Security** and allow this launch.

Sigla 1.0 Public Preview uses an ad-hoc signature with hardened runtime and has not completed Apple notarization.

### Update

Sigla 1.0 does not update itself. Quit Sigla, download the latest DMG, then replace the existing `Sigla.app` in Applications. Private application data continues to use the same bundle identifier.

### Quit and background behavior

- The red window button hides Sigla while the app continues running in the Dock and menu bar.
- Click the Dock icon or menu-bar icon to restore the window.
- Use `Command-Q`, the application menu, the Dock menu, or **Quit Sigla** in the menu bar to end the process.

### Uninstall

1. Quit Sigla completely.
2. Move `/Applications/Sigla.app` to Trash.
3. To remove private state as well, delete:
   - `~/Library/Application Support/com.zhoupeng.agentmarkdownreader`
   - `~/Library/Caches/com.zhoupeng.agentmarkdownreader`
   - `~/Library/WebKit/com.zhoupeng.agentmarkdownreader`
   - `~/Library/Preferences/com.zhoupeng.agentmarkdownreader.plist`
4. Delete the corresponding entry under `com.zhoupeng.sigla.ai-credentials` in Keychain Access, or remove the API key from Sigla before uninstalling.

Steps 3 and 4 permanently remove local annotations, history, preferences, and credentials.

### Ask for help

Use [GitHub Issues](https://github.com/z18520736823-coder/sigla-desktop/issues/new?template=bug.yml) and include:

- Sigla version
- macOS version
- Apple Silicon or Intel
- Reproduction steps
- A screenshot with private content removed

Never submit an API key, a complete private path, or confidential Markdown.

## 简体中文

### 安装

1. 从[公开预览版 Release](https://github.com/z18520736823-coder/sigla-desktop/releases/tag/v1.0.0-preview.1)下载 `Sigla_1.0.0_universal.dmg`。
2. 确认 SHA-256 为 `eb47705320e80943b916e430e4dd3cc3b370c0caf56a8b53cbd132c0cd961ecc`。
3. 打开 DMG，将 Sigla 拖入“应用程序”。
4. 首次启动请前往 **Finder → 应用程序**，按住 Control 点击 Sigla 并选择“打开”。
5. 如 macOS 继续拦截，请前往 **系统设置 → 隐私与安全性** 允许本次打开。

Sigla 1.0 公开预览版采用 ad-hoc 签名并启用 hardened runtime，尚未完成 Apple 公证。

### 更新

Sigla 1.0 不会自动更新。退出 Sigla，下载最新 DMG，再替换“应用程序”中的 `Sigla.app`。应用私有数据继续沿用同一 bundle identifier。

### 退出与后台运行

- 点击红色关闭按钮会隐藏窗口，Sigla 继续在 Dock 与顶部菜单栏运行。
- 点击 Dock 图标或顶部菜单栏图标可恢复窗口。
- 使用 `Command-Q`、应用菜单、Dock 菜单或状态栏中的“退出 Sigla”可完全结束进程。

### 卸载

1. 完全退出 Sigla。
2. 将 `/Applications/Sigla.app` 移到废纸篓。
3. 如需同时删除私有状态，可移除：
   - `~/Library/Application Support/com.zhoupeng.agentmarkdownreader`
   - `~/Library/Caches/com.zhoupeng.agentmarkdownreader`
   - `~/Library/WebKit/com.zhoupeng.agentmarkdownreader`
   - `~/Library/Preferences/com.zhoupeng.agentmarkdownreader.plist`
4. 在“钥匙串访问”中删除 `com.zhoupeng.sigla.ai-credentials` 下对应项目，或在卸载前通过 Sigla 设置删除 API Key。

第 3、4 步会永久删除本地批注、历史、偏好和凭据。

### 获取帮助

通过 [GitHub Issues](https://github.com/z18520736823-coder/sigla-desktop/issues/new?template=bug.yml) 提交：

- Sigla 版本
- macOS 版本
- Apple 芯片或 Intel
- 复现步骤
- 已移除私人内容的截图

请勿提交 API Key、完整私人路径或机密 Markdown。
