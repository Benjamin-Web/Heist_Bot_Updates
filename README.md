<p align="center">
  <img src="https://raw.githubusercontent.com/Benjamin-Web/heist_bot/main/renderer/assets/heist-icon.png" alt="Heist Bot Logo" width="120" height="120" style="border-radius: 20px;" />
</p>

<h1 align="center">Heist Bot</h1>

<p align="center">
  <strong>The All-in-One Twitch Stream Management Platform</strong><br/>
  <sub>Interactive games · Chat moderation · Custom commands · Timer automation · One-click Twitch login</sub>
</p>

<p align="center">
  <a href="https://github.com/Benjamin-Web/Heist_Bot_Updates/releases/latest"><img src="https://img.shields.io/github/v/release/Benjamin-Web/Heist_Bot_Updates?style=for-the-badge&color=9146ff&label=Download" alt="Latest Release" /></a>
  <img src="https://img.shields.io/badge/platform-Windows-0078D6?style=for-the-badge&logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/license-ISC-green?style=for-the-badge" alt="License" />
</p>

<p align="center">
  <a href="https://www.heist-bot.pro">🌐 Website</a> •
  <a href="https://discord.gg/FV83Fcu3V3">💬 Discord</a> •
  <a href="https://ko-fi.com/ronincannons">☕ Ko-fi / PRO</a>
</p>

---

## 🚀 What is Heist Bot?

Heist Bot is a **professional desktop application** for Twitch streamers that replaces multiple tools in one package. Run interactive heist games, moderate your chat, set up custom commands, automate timed messages — all from a single, beautiful dashboard.

> **No more juggling StreamElements, Nightbot, and separate bots.** Heist Bot handles it all.

---

## ⚡ Download & Install

1. **Download** the latest **[HeistBot-Setup-1.5.1.exe](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases/latest)** from the Releases page
2. **Run** the installer and follow the setup wizard
3. **Launch** Heist Bot and click **"Login with Twitch"**
4. You're live! 🎉

> The app checks for updates automatically on every launch. You'll be notified when a new version is available.

---

## ✨ Core Features

### 🎮 Interactive Heist Game
Viewers pool their currency and rob banks together. Win big or lose it all — with full animated OBS overlay, sound effects, and a dynamic robber parade.

### 🔐 One-Click Twitch Login
No more copy-pasting OAuth tokens. Click **"Login with Twitch"**, authorize, done. Channel, token, and Helix API are auto-configured.

### 🛡️ Chat Moderation (Spam Filter)
Built-in protection against caps spam, emoji floods, repeated messages, and links from non-subscribers. Fully configurable thresholds and timeouts.

### ⌨️ Custom Chat Commands
Create unlimited custom commands (`!discord`, `!socials`, `!ad`, etc.) with support for text responses, URLs, and sound alerts.

### ⏱️ Timer Commands
Automated recurring chat messages at custom intervals. Perfect for promoting Discord, social media, or game commands — no external tool needed.

### 🎫 Raffle System
Run fair giveaways with ticket pricing, sub-only mode, minimum subscription requirements, and automatic redraw on unclaimed wins.

### 📊 Statistics Dashboard
Track heist win rates, participation trends, raffle history, and top winners with interactive charts and filters.

### 🧟 Zombie Dog Mode
An alternative game mode where zombie dogs attack a sausage factory. Different mechanics, custom Spine animations, and a unique theme.

### 🌍 5 Languages
Full localization for **German**, **English**, **Spanish**, **Russian**, and **Chinese** — switchable with one click.

### 💰 Loyalty System
Automatic currency rewards for watch time and subscriptions (Tier 1, 2 & 3). Viewers earn, bet, and compete.

### 🚀 Auto-Updates
The bot automatically checks for updates at startup and guides you through one-click installs.

---

## 🛠️ Setup Guide

### OBS Overlay
1. Add a **Browser Source** in OBS
2. Set the URL to `http://localhost:8765/?lang=en` (or `?lang=de` for German)
3. Resolution: **1920 × 1080**
4. ✅ Enable "Control audio via OBS"

### Spam Filter
Configure directly in the **Settings** tab of the dashboard:

| Setting | Default | Description |
|---------|---------|-------------|
| Max Caps | 70% | Uppercase threshold before timeout |
| Max Emojis | 8 | Maximum emojis per message |
| Repeat Threshold | 3 | Identical messages within time window |
| Link Block | On | Block links from non-subscribers |

---

## 🎮 Chat Commands

| Command | Aliases | Description |
|---------|---------|-------------|
| `!raub <bet>` | `!heist <bet>` | Start or join a bank heist |
| `!coins` | `!<currency>` | Check your balance |
| `!topliste` | `!leaderboard` | Show top 5 in chat |
| `!give @user <amount>` | — | Transfer currency to another viewer |
| `!top` | — | (Mod) Show top 10 leaderboard |
| `!heistbot` | `!raubbot` | Show bot version info |

---

## ⭐ PRO Membership

Unlock the full potential of Heist Bot with PRO.

| Feature | Free | PRO |
|---------|:----:|:---:|
| Heist Game & OBS Overlay | ✅ | ✅ |
| Loyalty System | ✅ | ✅ |
| Spam Filter | ✅ | ✅ |
| Timer Commands | ✅ | ✅ |
| One-Click Twitch Login | ✅ | ✅ |
| Custom Commands | — | ✅ |
| Excluded Accounts | — | ✅ |
| Advanced Statistics | — | ✅ |
| Zombie Dog Mode | — | ✅ |
| Visual Polls | — | ✅ |
| Heist Cooldown Config | — | ✅ |
| Priority Support | — | ✅ |

### How to Activate PRO
1. Visit **[ko-fi.com/ronincannons](https://ko-fi.com/ronincannons)**
2. Purchase the **"Heist Bot PRO"** membership
3. Enter `Twitch: YourUsername` in the Order Note field
4. PRO activates automatically within minutes ✅

---

## 📝 Changelog

### [1.5.1] — 2026-05-15  ·  _"The Independence Update"_

This release transforms Heist Bot from a heist-only game bot into a **complete stream management platform**. Streamers no longer need StreamElements or Nightbot for basic moderation, custom commands, and timed messages — Heist Bot now handles all of this natively.

#### ✨ New Features
- **One-Click Twitch Login** — StreamElements-style managed OAuth. Click "Login with Twitch", authorize, done. Channel name, token, and Helix API are auto-configured. No more manual OAuth token generation.
- **Spam Filter** — Built-in chat moderation engine with configurable protection against caps spam, emoji floods, repeated messages, and links from non-subscribers. Timeouts are applied automatically.
- **Custom Chat Commands** — Create unlimited custom commands (`!discord`, `!ad`, `!socials`, etc.) with support for text, URL, and sound response types. Managed through the PRO dashboard.
- **Timer / Auto-Messages** — Automated recurring chat messages at configurable intervals (1–1440 minutes). Perfect for promoting Discord, social media, or game commands on autopilot.
- **Twitch Helix API for All Users** — The Helix API integration (EventSub, broadcaster info, shoutouts) is now available for all users, no longer PRO-exclusive.
- **Twitch SSO Token Exchange** — New backend endpoint for secure Twitch-to-JWT token exchange, enabling single-source-of-truth authentication across the app and backend.

#### 🔧 Improvements
- **Persistent Login State** — The header now correctly displays your Twitch username after app restart, without requiring re-authentication.
- **Cleaner Settings UI** — Manual channel/token input fields are now hidden under a collapsible "Advanced" section. Most users will never need them thanks to One-Click Login.
- **Exception Hardening** — Comprehensive try/catch wrappers across all new modules (bot, main process, renderer, timer service) to prevent unhandled crashes.
- **OAuth Redirect-URI Fixes** — Resolved Twitch redirect mismatch errors for the managed login flow.
- **Synchronized Auth State** — Login state in the header, settings card, and auth modal are now kept in sync from every possible entry point (OAuth, manual connect, app restart).

#### 🐛 Bug Fixes
- **Header Username Missing on Restart** — Fixed a `data-i18n` attribute conflict where the i18n system would overwrite the logged-in username with the generic "Login" label after the auth UI had already set it.
- **Shoutout Without Helix** — The shoutout command no longer crashes when the Helix API is unavailable.

---

### [1.4.5] — 2026-05-07
#### 🐛 Fixed
- **Zombie Dog Game Mode:** Fixed Spine animations getting stuck in the Joining phase on certain skins.
- **OBS Overlay Cleanup:** Fixed orphaned Spine animations on robbery resolution.

### [1.4.0] — 2026-05-02
#### ✨ Added
- Live configuration updates without restart.
- Self-healing PRO activation for missing database records.

#### 🐛 Fixed
- Case-insensitive user lookup for PRO activation.
- Email normalization during registration and login.

---

## 🗺️ Roadmap

| Status | Feature |
|:------:|---------|
| ✅ | Interactive Heist Game with OBS Overlay |
| ✅ | Raffle System (Sub-Only, Redraw, Claim Timer) |
| ✅ | Statistics Dashboard with Trends & Charts |
| ✅ | 5 Languages (DE, EN, ZH, ES, RU) |
| ✅ | PRO Membership System (Ko-fi Integration) |
| ✅ | Zombie Dog Game Mode |
| ✅ | Visual Polls & Tug-of-War |
| ✅ | Twitch Helix API Integration |
| ✅ | **One-Click Twitch OAuth Login** |
| ✅ | **Spam Filter (Caps, Emojis, Links, Repeats)** |
| ✅ | **Custom Chat Commands** |
| ✅ | **Timer / Auto-Messages** |
| 🔜 | Enhanced Heist Effects & Animations |
| 🔜 | Additional Game Modes |
| 🔜 | Deep EventSub Channel Points Integration |
| 🔜 | Context-Aware AI Chat Responses |

---

## 🤝 Support & Community

Having issues or feature requests? Join our community:

<p align="center">
  <a href="https://discord.gg/FV83Fcu3V3">
    <img src="https://img.shields.io/badge/Join-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" />
  </a>
  <a href="https://ko-fi.com/ronincannons">
    <img src="https://img.shields.io/badge/Support_on-Ko--fi-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white" alt="Ko-fi" />
  </a>
</p>

---

## 📄 License

This project is licensed under the **ISC License**.

---

<p align="center">
  <sub>Developed with ❤️ for the Twitch community by <a href="https://github.com/Benjamin-Web">Benjamin-Web</a></sub>
</p>
