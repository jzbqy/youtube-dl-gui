<img src="https://raw.githubusercontent.com/jely2002/youtube-dl-gui/v2.0.0/renderer/img/icon.png" alt="logo" align="left" height="100"/>

# Open Video Downloader (youtube-dl-gui) <br> ![version badge](https://img.shields.io/github/v/release/jzbqy/youtube-dl-gui?label=latest-release) ![GitHub](https://img.shields.io/github/license/jely2002/youtube-dl-gui) ![downloads](https://img.shields.io/github/downloads/jzbqy/youtube-dl-gui/total)
[https://jely2002.github.io/youtube-dl-gui](https://jely2002.github.io/youtube-dl-gui)

**[简体中文](README.md)** | **[English](README.en.md)**

## 中文定制版

此版本已添加完整的简体中文支持：
- 默认语言设置为简体中文
- 使用中国大陆习惯的中文用词（视频、音频、播放列表等）
- 完整的简体中文界面支持

---

## 关于此复刻

本仓库是 [jely2002/youtube-dl-gui](https://github.com/jely2002/youtube-dl-gui) 的简体中文定制版。

感谢原作者 [Jelle Gleed](https://github.com/jely2002) 开发的优秀项目！

### 主要修改
- 添加完整的简体中文翻译
- 默认语言设置为简体中文
- 使用中国大陆习惯的中文用词（视频、音频、播放列表等）

### 关于构建版本

此复刻版本**目前仅提供 Windows 平台**的构建版本，原因如下：

1. **签名证书要求**：
   - macOS 应用必须经过 Apple 签名和公证才能正常运行
   - Windows 应用签名可以避免 SmartScreen 安全警告
   - 获得这些签名需要付费的开发者账号（Apple $99/年，Windows 签名证书约 $200+/年）

2. **其他平台的可替代方案**：
   - **macOS 和 Linux 用户**：可以直接复刻此仓库到自己的 GitHub 账号，利用 GitHub Actions 免费构建服务
   - 复刻后，只需在仓库 Settings → Secrets 中添加必要的签名密钥（如果有），即可自动构建
   - 具体构建步骤可参考原项目的 CONTRIBUTING.md

3. **保留完整的自动更新功能**：
   - Windows 版本保留了完整的自动更新功能
   - 使用原作者的签名密钥配置，可正常接收更新

如需其他平台的官方签名版本，请使用 [原作者的官方版本](https://github.com/jely2002/youtube-dl-gui/releases)。

---

Open Video Downloader 是一个简单的跨平台桌面应用程序，让你可以从数百个支持的网站下载视频、音频、字幕和元数据，不仅仅是 YouTube。
它围绕 [yt-dlp](https://github.com/yt-dlp/yt-dlp) 提供了一个易于使用的界面，所以你不必接触命令行。

## 功能特性

- **跨平台:** 支持 Windows、macOS 和 Linux。
- **音频或视频下载:** 下载完整视频或仅提取音轨。
- **字幕和元数据:** 自动保存可用的字幕和视频信息。
- **画质控制:** 选择你偏好的分辨率、帧率和输出格式（如 MP4 或 MKV）。
- **播放列表:** 一键下载整个播放列表。
- **自定义输出:** 设置下载位置，并使用预设或自定义模板控制文件名。
- **智能队列:** OVD 自动平衡多个下载任务，不会让你的电脑变慢。
- **认证支持:** 支持浏览器 Cookie 文件、基本认证和视频密码。
- **自动更新:** 应用程序和 yt-dlp 都会自动保持最新。
- **明暗主题:** 适应系统主题，提供清晰的进度和错误处理。
- **快捷键:** 使用快捷键添加队列和下载视频，通过通知保持最新进度。

## 下载

适用于 **Windows** 的最新版本可在
[GitHub Releases 页面](https://github.com/jzbqy/youtube-dl-gui/releases) 获取。

#### 我应该下载哪个文件？
| 你的电脑 | 下载文件 |
|---------|----------|
| **Windows 安装版** | `Open.Video.Downloader_x.x.x_x64-setup.exe` |
| **Windows 便携版** | `Open.Video.Downloader_x.x.x_x64-portable.zip` |

## 工作原理

Open Video Downloader 使用 Vue 3 构建的前端和由 [Tauri](https://tauri.app/) 驱动的 Rust 后端。
当你添加视频或播放列表时，应用程序与 yt-dlp 通信以获取信息、处理选项并开始下载。
下载进度和任何错误都会显示在应用程序中。

## 贡献

欢迎开发者贡献代码。
你需要安装 Node.js (v24+) 和 Rust。

```
npm install
npm run tauri dev
```

有关更多详情，请参见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 许可证和免责声明

Open Video Downloader 根据 [AGPL-3.0 许可证](./LICENSE) 分发。

#### 负责任地使用此应用程序
如 AGPL-3.0 许可证（第 16 节）所述，Open Video Downloader 的维护者不对此应用程序的滥用承担责任。
我们不赞成使用本软件违反当地法律或平台服务条款（包括 DMCA）。
用户个人有责任确保公平和在法律范围内使用本软件。