<div align="center">

# VEGA SOUND

### Telegram Group Voice Chat Music Bot

A feature-rich Telegram music bot built with Python, Pyrogram, and PyTgCalls.

<p>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Platform-Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

</div>

---

## Overview

**VEGA SOUND** is a Telegram music bot project designed to play audio in group voice chats. It combines multiple music sources, playback controls, queue management, inline interfaces, and administrative tools in one project.

The codebase is organized into platform integrations, playback plugins, bot utilities, and configuration modules.

## Features

### Music Playback
- Play music and audio in Telegram group voice chats.
- Search for tracks and process supported music links.
- Support for YouTube, Spotify, SoundCloud, Apple Music, Resso, and Telegram media integrations.
- Audio streaming and track downloading utilities.
- Display track information and thumbnails where supported.
- Queue-based playback for managing upcoming tracks.

### Playback Controls
- Pause and resume the current track.
- Skip to the next track.
- Stop playback.
- Seek to a selected position.
- Adjust playback speed.
- Shuffle the queue.
- Repeat or loop playback.
- View and manage the current queue.

### Bot Interface
- Start and help menus.
- Inline buttons and callback interactions.
- Interactive playback and settings panels.
- Configurable bot commands.
- Track and playlist information displays.

### Administration
- Admin authorization and permission checks.
- Group playback controls.
- Owner and privileged-user configuration.
- Broadcast and assistant-management utilities.
- Automatic assistant leave settings.

### Storage and Utilities
- MongoDB integration through Motor.
- Local JSON-based storage support.
- Logging and runtime statistics utilities.
- Thumbnail and media-processing helpers.
- Cookie and download support utilities.

## Supported Integrations

| Platform | Integration |
|---|---|
| YouTube | Search, track processing, and playback |
| Spotify | Track and playlist-related processing |
| SoundCloud | Audio source integration |
| Apple Music | Music link integration |
| Resso | Music source integration |
| Telegram | Audio and video media |

*Actual availability may depend on external services, API access, cookies, and the configuration supplied by the operator.*

## Project Structure

```text
VEGA-SOUND/
├── Make/
│   ├── VeGa/
│   │   ├── core/          # Bot, userbot, and database core
│   │   ├── platforms/     # Music platform integrations
│   │   ├── plugins/
│   │   │   ├── admins/    # Playback and admin controls
│   │   │   ├── bot/       # Start, help, inline, and settings
│   │   │   ├── misc/      # Utility features
│   │   │   └── play/      # Playback and music commands
│   │   ├── utils/         # Helpers, queues, streams, and tools
│   │   └── assets/        # Images, fonts, and media assets
│   ├── config.py          # Configuration settings
│   ├── requirements.txt  # Make package dependencies
│   └── sample.env         # Environment variable template
├── Maker/                 # Additional bot modules
├── bot.py                 # Bot startup module
├── main.py                # Main launcher
├── requirements.txt       # Python dependencies
├── setup                  # Linux dependency installer
└── start                  # Startup script
```

## Requirements

- Python 3
- FFmpeg
- Telegram API ID and API Hash
- Telegram Bot Token
- MongoDB connection URI (for database-backed features)
- A Telegram account session for assistant/userbot functionality, where required
- Required API credentials and cookies for integrations that need them

## Configuration

1. Create a Telegram application at [my.telegram.org](https://my.telegram.org) to obtain your `API_ID` and `API_HASH`.
2. Create a bot with [@BotFather](https://t.me/BotFather) to obtain your bot token.
3. Prepare a MongoDB connection URI if you intend to use database-backed features.
4. Review `Make/sample.env` and the configuration modules.
5. Supply your own credentials through environment variables or a secure configuration method.

Common configuration variables include:

| Variable | Purpose |
|---|---|
| `API_ID` | Telegram API ID |
| `API_HASH` | Telegram API Hash |
| `BOT_TOKEN` | Telegram bot token |
| `OWNER_ID` | Bot owner Telegram user ID |
| `LOGGER_ID` | Logging chat ID |
| `MONGO_DB_URI` | MongoDB connection URI |
| `STRING_SESSION` | Assistant account session |
| `COOKIE_URL` | Cookie source, when required |
| `API_URL` / `API_KEY` | Optional external API settings |

**Security:** Never publish bot tokens, API secrets, session strings, database credentials, or private cookies. If any real credentials have been committed to a repository, revoke or rotate them before deploying. Keep secrets in environment variables and remove hard-coded credentials from source files.

## Installation

Clone the repository:

```bash
git clone <YOUR_REPOSITORY_URL>
cd VEGA-SOUND
```

Install system dependencies on Debian/Ubuntu:

```bash
sudo apt update
sudo apt install -y python3 python3-pip ffmpeg
```

Install Python packages:

```bash
pip install -r requirements.txt
```

Configure the required environment variables, then review the startup modules and launch command for your deployment environment.

> **Important:** This repository contains more than one startup/configuration path. Verify the intended entry point and ensure that all required settings are loaded from your environment before running it. The included files may require adjustment for your hosting platform.

## Deployment Notes

- Keep FFmpeg installed and available in the system `PATH`.
- Use a stable host that supports persistent Python processes and Telegram voice-chat connections.
- Configure MongoDB and any required external API credentials.
- Check platform/API restrictions and keep dependencies compatible.
- Monitor logs for download, streaming, and connection errors.

## License

This project includes a `LICENSE` file. Review that file for the applicable license terms before copying, modifying, or redistributing the code.

## Credits

Developed and customized under the **VEGA SOUND** project identity.

For support, updates, and project information, use the official links provided by the project owner.

---

<div align="center">

**VEGA SOUND**  
*Music • Voice Chats • Telegram*

</div>

<!-- ═══════════════════════════════════════════════════════════════════════ --><!--                       Copyright | Footer                              --><!-- ═══════════════════════════════════════════════════════════════════════ --><div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:3B82F6,100:0F172A&height=4&width=40%&section=header" />
  <br><br>  <p style="color: #9CA3AF; font-size: 14px;">
    <b style="color: #3B82F6;">Brand:</b> VEGA &amp; Logic &nbsp;|&nbsp;
    <b style="color: #3B82F6;">Copyright:</b> © 2015 - 2025
  </p>
  <p style="color: #6B7280; font-size: 12px;">
  </p>
</div><br><!-- Smooth Gradient Footer Background --><img src="https://capsule-render.vercel.app/api?type=waving&color=0:3B82F6,50:1E3A8A,100:0F172A&height=120&section=footer" width="100%" /></div>
