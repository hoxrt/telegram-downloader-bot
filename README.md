# 🤖 Telegram Video Downloader Bot

A Telegram bot that downloads videos from **X (Twitter)** and sends them straight back to the chat. Just send a link — the bot handles the rest.

> 🔒 **Showcase repository.** The source code is private. If you're a recruiter or company and would like to review the code, feel free to contact me and I'll grant access.

---

## ✨ Features

- 🔗 **Paste and go** — send an X/Twitter link, get the video back in seconds
- 🛡️ **Reliable downloads** — multiple download strategies with automatic fallback if one fails
- 🧹 **Clean chat** — the bot automatically removes the status message and the original link after delivery
- ⚡ **Live status updates** — the user sees progress while the video is being prepared
- ☁️ **Always online** — deployed in the cloud and running 24/7

---

## 🛠️ Tech Stack

| Area | Technology |
|---|---|
| Runtime | Node.js |
| Bot framework | node-telegram-bot-api |
| Video processing | yt-dlp, ffmpeg |
| Configuration | Environment variables (dotenv) |
| Hosting | Railway (auto-deploy from GitHub) |

---

## ⚙️ How It Works

```
User sends a link
       │
       ▼
Validate the link
       │
       ▼
Try primary download method ──✗──► Fallback method(s)
       │                                   │
       ✓                                   ✓
       ▼                                   ▼
Send video to the user, then clean up the chat
```

---

## 🧩 Challenges I Solved

- **Bot conflicts (HTTP 409):** diagnosed and fixed conflicts caused by multiple bot instances polling at the same time.
- **Cross-platform commands:** made the bot run the same way on Windows (local development) and Linux (cloud).
- **Secure configuration:** kept the bot token and all secrets out of the codebase using environment variables.

---

## 🗺️ Roadmap

- [x] X (Twitter) video downloads
- [x] Automatic chat cleanup after delivery
- [ ] YouTube support (videos & Shorts)
- [ ] TikTok support
- [ ] Quality selection before downloading

---

## 👤 About Me

**Yahya Alfaifi** — Full Stack Developer based in Riyadh, Saudi Arabia.

- GitHub: [@hoxrt](https://github.com/hoxrt)
- LinkedIn: [yahya-alfaifi](https://www.linkedin.com/in/yahya-alfaifi-a49740385)
- Email: yahya.alfaifi131@gmail.com

---

© 2026 Yahya Alfaifi. All rights reserved.
