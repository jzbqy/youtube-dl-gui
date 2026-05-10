<img src="https://raw.githubusercontent.com/jely2002/youtube-dl-gui/v2.0.0/renderer/img/icon.png" alt="logo" align="left" height="100"/>

# Open Video Downloader (youtube-dl-gui) <br> ![version badge](https://img.shields.io/github/v/release/jzbqy/youtube-dl-gui?label=latest-release) ![GitHub](https://img.shields.io/github/license/jely2002/youtube-dl-gui) ![downloads](https://img.shields.io/github/downloads/jzbqy/youtube-dl-gui/total)
[https://jely2002.github.io/youtube-dl-gui](https://jely2002.github.io/youtube-dl-gui)

**[简体中文](README.md)** | **[English](README.en.md)**

## Simplified Chinese Version

This version includes complete Simplified Chinese support:
- Default language set to Simplified Chinese
- Uses Chinese vocabulary习惯 (video, audio, playlist, etc.)
- Complete Simplified Chinese interface support

---

## About This Fork

This repository is a Simplified Chinese localized version of [jely2002/youtube-dl-gui](https://github.com/jely2002/youtube-dl-gui).

Special thanks to the original author [Jelle Gleed](https://github.com/jely2002) for developing this excellent project!

### Main Changes
- Added complete Simplified Chinese translation
- Default language set to Simplified Chinese
- Uses Simplified Chinese vocabulary习惯 (video, audio, playlist, etc.)

### About Build Targets

This fork currently provides builds **only for the Windows platform** for the following reasons:

1. **Signing Certificate Requirements**:
   - macOS applications must be signed and notarized by Apple to run properly
   - Windows application signing helps avoid SmartScreen security warnings
   - Obtaining these signatures requires paid developer accounts (Apple $99/year, Windows signing certificates ~$200+/year)

2. **Alternative Solutions for Other Platforms**:
   - **macOS and Linux users**: Can directly fork this repository to their own GitHub account and use GitHub Actions for free builds
   - After forking, simply add the necessary signing keys (if available) in repository Settings → Secrets for automatic builds
   - See the original project's CONTRIBUTING.md for detailed build instructions

3. **Preserved Full Auto-Update Functionality**:
   - Windows version retains complete auto-update functionality
   - Uses the original author's signing key configuration for normal update reception

For official signed versions on other platforms, please use the [original author's official release](https://github.com/jely2002/youtube-dl-gui/releases).

---

Open Video Downloader is a simple cross-platform desktop application that allows you to download videos, audio, subtitles and metadata from hundreds of supported websites, not just YouTube.
It provides an easy-to-use interface around [yt-dlp](https://github.com/yt-dlp/yt-dlp), so you don't have to touch the command line.

## Features

- **Cross-platform:** Supports Windows, macOS and Linux.
- **Audio or video downloads:** Download full videos or extract audio tracks only.
- **Subtitles and metadata:** Automatically save available subtitles and video information.
- **Quality control:** Choose your preferred resolution, framerate and output format (e.g. MP4 or MKV).
- **Playlists:** Download entire playlists with one click.
- **Custom output:** Set download location and control file names with preset or custom templates.
- **Smart queuing:** OVD automatically balances multiple downloads so your computer doesn't slow down.
- **Authentication support:** Supports browser cookie files, basic authentication and video passwords.
- **Auto-updates:** Both the application and yt-dlp are automatically kept up to date.
- **Light and dark theme:** Adapts to your system theme with clear progress and error handling.
- **Shortcuts:** Use shortcuts to add to queue and download videos, with notifications to keep you updated on progress.

## Downloads

The latest version for **Windows** is available on the
[GitHub Releases page](https://github.com/jzbqy/youtube-dl-gui/releases).

#### Which file should I download?
| Your computer | Download file |
|-------------|--------------|
| **Windows Installer** | `Open.Video.Downloader_x.x.x_x64-setup.exe` |
| **Windows Portable** | `Open.Video.Downloader_x.x.x_x64-portable.zip` |

## How It Works

Open Video Downloader uses a Vue 3 built frontend and a Rust backend powered by [Tauri](https://tauri.app/).
When you add a video or playlist, the application communicates with yt-dlp to get information, process options and start downloading.
Download progress and any errors are shown in the application.

## Contributing

Developers are welcome to contribute code.
You will need Node.js (v24+) and Rust installed.

```
npm install
npm run tauri dev
```

See [CONTRIBUTING.md](./CONTRIBUTING.md) for more details.

## License and Disclaimer

Open Video Downloader is distributed under the [AGPL-3.0 license](./LICENSE).

#### Use this application responsibly
As stated in section 16 of the AGPL-3.0 license, the maintainers of Open Video Downloader are not responsible for any misuse of this application.
We do not condone using this software to violate local laws or platform terms of service (including DMCA).
It is the user's personal responsibility to ensure fair use and use within legal boundaries.