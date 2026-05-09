<img src="https://raw.githubusercontent.com/jely2002/youtube-dl-gui/v2.0.0/renderer/img/icon.png" alt="logo" align="left" height="100"/>

# Open Video Downloader (youtube-dl-gui)  ![version badge](https://img.shields.io/github/v/release/jely2002/youtube-dl-gui?label=latest-release) ![GitHub](https://img.shields.io/github/license/jely2002/youtube-dl-gui) ![downloads](https://img.shields.io/github/downloads/jely2002/youtube-dl-gui/total)

<https://jely2002.github.io/youtube-dl-gui>

**[简体中文](README.md)** | **[English](README.en.md)**

## 中文定制版

此版本已添加完整的简体中文支持：

- 默认语言设置为简体中文
- 使用中国大陆习惯的中文用词（视频、音频、播放列表等）
- 完整的简体中文界面支持

***

Open Video Downloader 是一个简单的跨平台桌面应用程序，让你可以从数百个支持的网站下载视频、音频、字幕和元数据，不仅仅是 YouTube。\
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

适用于 **Windows**、**macOS** 和 **Linux** 的最新版本可在\
[GitHub Releases 页面](https://github.com/jzbqy/youtube-dl-gui/releases) 获取。

下载适合你平台的安装程序或压缩包，然后按照正常的安装步骤进行。\
无需命令行设置。

#### 我应该下载哪个文件？

| 你的电脑                                  | 下载文件                                           |
| ------------------------------------- | ---------------------------------------------- |
| **Windows**                           | `Open.Video.Downloader_x.x.x_x64-setup.exe`    |
| **Windows 便携版**                       | `Open.Video.Downloader_x.x.x_x64-portable.zip` |
| **Mac (Intel)**                       | `Open.Video.Downloader_x.x.x_x64.dmg`          |
| **Mac (Apple Silicon – M1, M2 … M5)** | `Open.Video.Downloader_x.x.x_aarch64.dmg`      |
| **Linux 通用 (x64)**                    | `Open.Video.Downloader_x.x.x_amd64.AppImage`   |
| **Linux 通用 (aarch64)**                | `Open.Video.Downloader_x.x.x_aarch64.AppImage` |
| **Linux Debian/Ubuntu (x64)**         | `Open.Video.Downloader_x.x.x_amd64.deb`        |
| **Linux Debian/Ubuntu (aarch64)**     | `Open.Video.Downloader_x.x.x_arm64.deb`        |
| **Linux Fedora/RHEL (x64)**           | `Open.Video.Downloader_x.x.x-x_amd64.rpm`      |
| **Linux Fedora/RHEL (aarch64)**       | `Open.Video.Downloader_x.x.x-x_aarch64.rpm`    |

## 工作原理

Open Video Downloader 使用 Vue 3 构建的前端和由 [Tauri](https://tauri.app/) 驱动的 Rust 后端。\
当你添加视频或播放列表时，应用程序与 yt-dlp 通信以获取信息、处理选项并开始下载。\
下载进度和任何错误都会显示在应用程序中。

## 贡献

欢迎开发者贡献代码。\
你需要安装 Node.js (v24+) 和 Rust。

```
npm install
npm run tauri dev
```

有关更多详情，请参见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 许可证和免责声明

Open Video Downloader 根据 [AGPL-3.0 许可证](./LICENSE) 分发。

#### 负责任地使用此应用程序

如 AGPL-3.0 许可证（第 16 节）所述，Open Video Downloader 的维护者不对此应用程序的滥用承担责任。\
我们不赞成使用本软件违反当地法律或平台服务条款（包括 DMCA）。\
用户个人有责任确保公平和在法律范围内使用本软件。
