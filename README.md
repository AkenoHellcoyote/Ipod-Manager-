# Linux iPod Manager 🎵

A Linux desktop application for managing music and audiobooks on older iPods.

The project is designed for **classic, non-iOS iPods** and aims to make it possible to manage them comfortably from Linux without relying on iTunes or a terminal.

## ✨ Features

- 🎵 Add MP3 music
- 📖 Add M4B audiobooks
- 🖼️ Import embedded cover artwork
- 🏷️ Read metadata automatically
- 🗑️ Delete individual tracks
- 🗑️ Delete all music
- 🗑️ Delete all audiobooks
- 🗑️ Delete all media
- 💾 Display iPod storage usage
- 🔍 Automatically find mounted iPods
- 🛡️ Compatibility checks before write operations
- 🖥️ Graphical interface for Linux

## 🎯 Project Goal

The goal is to create a modern Linux tool for **older iPods that are no longer well supported by modern software**.

In particular, the project aims to support as many **non-iOS iPod generations** as possible:

- iPod Classic
- iPod Video
- iPod mini
- iPod nano
- iPod shuffle

Support for different generations may require different backends.

## 🚫 Out of Scope

This project does not target devices using the iOS media system:

- iPhone
- iPad
- iPod touch

## 🧰 Technology

The current version uses:

- Python
- Tkinter
- C
- libgpod
- FFmpeg / FFprobe

The graphical interface is written in Python, while iPod database operations are handled by a native C backend using libgpod.

## 🐧 Installation

### Ubuntu / Debian / Zorin OS

Install the required packages:

```bash
sudo apt update
sudo apt install python3 python3-tk gcc pkg-config libgpod-dev libgdk-pixbuf-2.0-dev ffmpeg
./install.sh
After installation, start Linux iPod Manager from the application menu.
📦 Portable AppImage
The project also contains an AppImage build system.
The goal is to provide a simple download for users who do not want to install the development dependencies manually.
AppImage support is currently considered beta and is being tested on different Linux distributions.
⚠️ Important
This software modifies the iPod's music database.
Always keep a backup of important iPod data before testing new versions.
The project is still in active development and support for different iPod generations is being expanded.
🛠️ Current Status
Early beta
The application has been tested successfully with an iPod nano 3rd generation, including:
- MP3 music
- M4B audiobooks
- embedded artwork
- deletion of media
More iPod generations will be tested and supported over time.
🗺️ Roadmap
- [x] MP3 import
- [x] M4B audiobook import
- [x] Cover artwork
- [x] Track deletion
- [x] Bulk deletion
- [x] iPod detection
- [x] Compatibility checks
- [x] Linux installer
- [ ] Automatic model detection improvements
- [ ] Database backups
- [ ] Playlist management
- [ ] More iPod generations
- [ ] Improved AppImage distribution
🤝 Contributing
Contributions, testing, bug reports and ideas are welcome.
Especially useful are reports from people using different iPod generations.
If you have an older iPod that is not currently supported, please open an issue with the exact model and generation.
📜 License
GPL-3.0-only

