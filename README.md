# 🎵 TgMusicBot – Telegram Music Bot [![Stars](https://img.shields.io/github/stars/Maya12981/Music-bot?style=social)](https://github.com/Maya12981/Music-bot/stargazers)

**A high-performance Telegram Voice Chat Bot** for streaming music from YouTube, Spotify, JioSaavn, and more. Built with Python, Py-Tgcalls, and PyTdBot.

<p align="center">
  <!-- GitHub Stars -->
  <a href="https://github.com/Maya12981/Music-bot/stargazers">
    <img src="https://img.shields.io/github/stars/Maya12981/Music-bot?style=for-the-badge&color=black&logo=github" alt="Stars"/>
  </a>
  
  <!-- GitHub Forks -->
  <a href="https://github.com/Maya12981/Music-bot/network/members">
    <img src="https://img.shields.io/github/forks/Maya12981/Music-bot?style=for-the-badge&color=black&logo=github" alt="Forks"/>
  </a>

  <!-- Last Commit -->
  <a href="https://github.com/Maya12981/Music-bot/commits/AshokShau">
    <img src="https://img.shields.io/github/last-commit/Maya12981/Music-bot?style=for-the-badge&color=blue" alt="Last Commit"/>
  </a>

  <!-- Repo Size -->
  <a href="https://github.com/Maya12981/Music-bot">
    <img src="https://img.shields.io/github/repo-size/Maya12981/Music-bot?style=for-the-badge&color=success" alt="Repo Size"/>
  </a>

  <!-- Language -->
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Written%20in-Python-orange?style=for-the-badge&logo=python" alt="Python"/>
  </a>

  <!-- License -->
  <a href="https://github.com/Maya12981/Music-bot/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/Maya12981/Music-bot?style=for-the-badge&color=blue" alt="License"/>
  </a>

  <!-- Open Issues -->
  <a href="https://github.com/Maya12981/Music-bot/issues">
    <img src="https://img.shields.io/github/issues/Maya12981/Music-bot?style=for-the-badge&color=red" alt="Issues"/>
  </a>

  <!-- Pull Requests -->
  <a href="https://github.com/Maya12981/Music-bot/pulls">
    <img src="https://img.shields.io/github/issues-pr/Maya12981/Music-bot?style=for-the-badge&color=purple" alt="PRs"/>
  </a>

  <!-- GitHub Workflow CI -->
  <a href="https://github.com/Maya12981/Music-bot/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/Maya12981/Music-bot/code-fixer.yml?style=for-the-badge&label=CI&logo=github" alt="CI Status"/>
  </a>
</p>

<p align="center">
   <img src="https://raw.githubusercontent.com/Maya12981/Music-bot/master/.github/images/thumb.png" alt="thumbnail" width="320" height="320">
</p>

### 🔥 Live Bot: [@Zoroo_Music_Bot](https://t.me/Zoroo_Music_Bot)

---

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **🎧 Multi-Platform Support** | YouTube, Spotify, Apple Music, SoundCloud, JioSaavn |
| **📜 Playlist Management** | Queue system with auto-play |
| **🎛️ Advanced Controls** | Volume, loop, seek, skip, pause/resume |
| **🌐 Multi-Language** | English, Hindi, Spanish, Arabic support |
| **⚡ Low Latency** | Optimized with PyTgCalls |
| **🐳 Docker Ready** | One-click deployment |
| **🔒 Anti-Ban** | Cookie & API-based authentication |

---

## 🚀 Quick Deploy

[![Deploy on Heroku](https://img.shields.io/badge/Deploy%20on%20Heroku-430098?style=for-the-badge&logo=heroku)](https://heroku.com/deploy?template=https://github.com/Maya12981/Music-bot)

---

## 📦 Installation Methods


<details>

<summary><strong>📌 Docker Installation (Recommended) (Click to expand)</strong></summary>

### 🐳 Prerequisites
1. Install Docker:
   - [Linux](https://docs.docker.com/engine/install/)
   - [Windows/Mac](https://docs.docker.com/desktop/install/)

### 🚀 Quick Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/Maya12981/Music-bot.git && cd Music-Bot
   ```

### 🔧 Configuration
1. Prepare environment file:
   ```sh
   cp sample.env .env
   ```

2. Edit configuration (choose one method):
   - **Beginner-friendly (nano)**:
     ```sh
     nano .env
     ```
     - Edit values
     - Save: `Ctrl+O` → Enter → `Ctrl+X`

   - **Advanced (vim)**:
     ```sh
     vi .env
     ```
     - Press `i` to edit
     - Save: `Esc` → `:wq` → Enter

### 🏗️ Build & Run
1. Build Docker image:
   ```sh
   docker build -t Music-Bot .
   ```

2. Run container (auto-restarts on crash/reboot):
   ```sh
   docker run -d \
     --name Music-Bot \
     --env-file .env \
     --restart unless-stopped \
     Music-Bot
   ```

### 🔍 Monitoring
1. Check logs:
   ```sh
   docker logs -f Music-Bot
   ```
   (Exit with `Ctrl+C`)

### ⚙️ Management Commands
- **Stop container**:
  ```sh
  docker stop Music-Bot
  ```

- **Start container**:
  ```sh
  docker start Music-Bot
  ```

- **Update the bot**:
  ```sh
  docker stop Music-Bot
  docker rm Music-Bot
  git pull origin master
  docker build -t Music-Bot .
  docker run -d --name Music-Bot --env-file .env --restart unless-stopped tgmusicbot
  ```

</details>


<details>
<summary><strong>📌 Step-by-Step Installation Guide (Click to Expand)</strong></summary>

### 🛠️ System Preparation
1. **Update your system** (Recommended):
   ```sh
   sudo apt-get update && sudo apt-get upgrade -y
   ```

2. **Install essential tools**:
   ```sh
   sudo apt-get install git python3-pip ffmpeg tmux -y
   ```

### ⚡ Quick Setup
1. **Install UV package manager**:
   ```sh
   pip3 install uv
   ```

2. **Clone the repository**:
   ```sh
   git clone https://github.com/Maya12981/Music-Bot.git && cd TgMusicBot
   ```

### 🐍 Python Environment
1. **Create virtual environment**:
   ```sh
   uv venv
   ```

2. **Activate environment**:
   - Linux/Mac: `source .venv/bin/activate`
   - Windows (PowerShell): `.\.venv\Scripts\activate`

3. **Install dependencies**:
   ```sh
   uv pip install -e .
   ```

### 🔐 Configuration
1. **Setup environment file**:
   ```sh
   cp sample.env .env
   ```

2. **Edit configuration** (Choose one method):
   - **For beginners** (nano editor):
     ```sh
     nano .env
     ```
     - Edit values
     - Save: `Ctrl+O` → Enter → `Ctrl+X`

   - **For advanced users** (vim):
     ```sh
     vi .env
     ```
     - Press `i` to edit
     - Save: `Esc` → `:wq` → Enter

### 🤖 Running the Bot
1. **Start in tmux session** (keeps running after logout):
   ```sh
   tmux new -s musicbot
   tgmusic
   ```

   **Tmux Cheatsheet**:
   - Detach: `Ctrl+B` then `D`
   - Reattach: `tmux attach -t musicbot`
   - Kill session: `tmux kill-session -t musicbot`

### 🔄 After Updates
To restart the bot:
```sh
tmux attach -t musicbot
# Kill with Ctrl+C
tgmusic
```

</details>

---

## ⚙️ Configuration Guide

<details>
<summary><b>🔑 Required Variables (Click to expand)</b></summary>

| Variable | Description | How to Get |
|----------|-------------|------------|
| `API_ID` | Telegram App ID | [my.telegram.org](https://my.telegram.org/apps) |
| `API_HASH` | Telegram App Hash | [my.telegram.org](https://my.telegram.org/apps) |
| `TOKEN` | Bot Token | [@BotFather](https://t.me/BotFather) |
| `STRING1-10` | Pyrogram Sessions | [@String_Session_generte_bot](https://t.me/String_Session_generte_bot) |
| `MONGO_URI` | MongoDB Connection | [MongoDB Atlas](https://cloud.mongodb.com) |

</details>

---

## 🍪 Avoiding Bans

### Option 1: Premium API
```env
API_URL=https://tgmusic.fallenapi.fun
API_KEY=your-secret-key
```
📌 Get keys: [Contact @Mr_Roronoa_zoroo](https://t.me/Mr_Roronoa_zoroo) or [@FallenApiBot](https://t.me/Mr_Roronoa_zoroo)

### Option 2: Cookies
[![Cookie Guide](https://img.shields.io/badge/Guide-Read%20Here-blue?style=flat-square)](https://github.com/Maya12981/Music-bot/blob/master/cookies/README.md)

---

## 🤖 Bot Commands

| Command | Description |
|---------|-------------|
| `/play [query]` | Play music from supported platforms |
| `/skip` | Skip current track |
| `/pause` / `/resume` | Control playback |
| `/volume [1-200]` | Adjust volume |
| `/queue` | Show upcoming tracks |
| `/loop` | Enable/disable loop |

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

**Note:** Minor typo fixes will be closed. Focus on meaningful contributions.

---

## 📜 License

AGPL-3.0 © [AshokShau](https://github.com/Maya12981).  
[![License](https://img.shields.io/github/license/Maya12981/Music-bot?color=blue)](LICENSE)

---

## 💖 Support

Help keep this project alive!  
[![Telegram](https://img.shields.io/badge/Chat-Support%20Group-blue?logo=telegram)](https://t.me/Zoro_bots)  
[![Donate](https://img.shields.io/badge/Donate-Crypto/PayPal-ff69b4)](https://t.me/Zoro_bots)

---

## 🔗 Connect

[![GitHub](https://img.shields.io/badge/Follow-GitHub-black?logo=github)](https://github.com/Maya12981)  
[![Channel](https://img.shields.io/badge/Updates-Channel-blue?logo=telegram)](https://t.me/Zoro_bots)

---
