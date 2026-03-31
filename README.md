# 🦹‍♂️ Heist Bot

**Bankräuber für deinen Twitch-Stream.**

[Deutsch](#deutsch) | [English](#english)

---

<a name="deutsch"></a>

## Deutsch

Ein Twitch-Bot, der deinen Stream mit einem Banküberfall-Minispiel aufmischt. Zuschauer setzen ihre Kanal-Währung ein, schließen sich zusammen und hoffen, dass die Polizei nicht schneller ist. Dazu gibt's ein animiertes OBS-Overlay, ein Raffle-System und ein Dashboard zur Steuerung – alles in einer Electron-App.

---

### 🎮 Was kann der Bot?

**Heist-System**
- Zuschauer starten mit `!raub <Einsatz>` einen Banküberfall oder schließen sich an
- Je mehr Leute mitmachen, desto höher der Multiplikator – aber auch das Risiko
- Polizei-Umzingelung bei Niederlage, SEK-Einsatz inklusive
- 60 Sekunden Joining-Phase mit animierten Räuber-Charakteren im Overlay

**Raffle-System**
- Verlosungen direkt aus dem Dashboard starten
- Zuschauer kaufen mit `!ticket <Anzahl>` Lose
- Animierte Gewinnziehung im Overlay mit Claim-Mechanik
- Einstellbar: Ticket-Preis, Max-Tickets, Sub-only mit Mindest-Abo

**Overlay & Optik**
- Animierter Räuber-Lauf am unteren Bildschirmrand (22 verschiedene Skins!)
- Bank-Gebäude, Sirenen, Soundeffekte
- Konfetti bei Raffle-Gewinn, Polizei-Animation bei Heist-Niederlage
- Sauber transparent für OBS – einfach als Browser-Quelle einbinden

**Dashboard**
- Alles auf einen Blick: Heist-Status, Leaderboard, Event-Log
- Manuelle Währungsverteilung an einzelne Nutzer oder alle
- Sprache umschaltbar (DE/EN)
- Auto-Updates direkt in der App

**Währung & Treue**
- Automatische Watch-Time-Belohnung (alle 5 Min)
- Sub-Boni für Tier 1, 2 und 3
- Schenkfunktion zwischen Zuschauern (`!give`)
- Lokale SQLite-Datenbank – kein externer Server nötig

---

### 🚀 Installation

1. **Download** – Neueste `.exe` von den [Releases](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases) holen
2. **Installieren** – Setup starten, fertig
3. **Einrichten** – Bot öffnen, Kanal + OAuth-Token eingeben, verbinden
4. **OBS** – Browser-Quelle mit `http://localhost:8765/` hinzufügen (1920×1080)

OAuth-Token bekommst du auf [twitchtokengenerator.com](https://twitchtokengenerator.com/).

---

### 📋 Chat-Befehle

| Befehl | Beschreibung |
|---|---|
| `!raub <Einsatz>` | Banküberfall starten oder beitreten |
| `!ticket <Anzahl>` | Raffle-Tickets kaufen |
| `!coins` / `!münzen` | Kontostand anzeigen |
| `!topliste` | Top 5 Räuber |
| `!top` | Top 10 (nur Mods) |
| `!give @User <Betrag>` | Währung verschenken |
| `!heistbot` | Bot-Info & Version |

---

### 💻 Tech Stack

| | |
|---|---|
| App | Electron |
| Twitch | tmi.js |
| Animationen | Phaser 3 + GSAP |
| Datenbank | SQLite (better-sqlite3) |
| Updates | electron-updater |

---

### 🗺️ Roadmap

- [x] Heist-System mit dynamischen Multiplikatoren
- [x] Animiertes OBS-Overlay
- [x] Polizei-Umzingelung & SEK-Einsatz
- [x] Raffle-System mit Overlay-Animation
- [ ] Erweiterte Statistiken im Dashboard
- [ ] Custom Sound-Upload
- [ ] Weitere Overlay-Themes

---

### 🤝 Mitmachen & Support

- 🐛 Bug gefunden? → [Issue erstellen](https://github.com/Benjamin-Web/Heist_Bot_Updates/issues)
- 💬 Fragen? → [Discord Server](https://discord.gg/FV83Fcu3V3)
- ☕ Unterstützen? → [Ko-fi](https://ko-fi.com/benjaminweb)

---

*Aktuell: v1.3.5*

---
---

<a name="english"></a>

## English

A Twitch bot that spices up your stream with a bank robbery mini-game. Viewers bet their channel currency, team up, and hope the police don't show up first. Comes with an animated OBS overlay, a raffle system, and a control dashboard – all in one Electron app.

---

### 🎮 What can it do?

**Heist System**
- Viewers start a bank heist with `!raub <bet>` or join one in progress
- More participants = higher multiplier, but also higher risk
- Police surround animation on loss, SWAT intervention included
- 60-second joining phase with animated robber characters in the overlay

**Raffle System**
- Start giveaways directly from the dashboard
- Viewers buy tickets with `!ticket <amount>`
- Animated winner draw in the overlay with claim mechanic
- Configurable: ticket price, max tickets, sub-only with minimum sub months

**Overlay & Visuals**
- Animated robber parade at the bottom of the screen (22 different skins!)
- Bank building, sirens, sound effects
- Confetti on raffle win, police animation on heist loss
- Clean transparent background for OBS – just add as browser source

**Dashboard**
- Everything at a glance: heist status, leaderboard, event log
- Manual currency distribution to individual users or everyone
- Language toggle (DE/EN)
- Auto-updates built right in

**Currency & Loyalty**
- Automatic watch-time rewards (every 5 min)
- Sub bonuses for Tier 1, 2, and 3
- Gift system between viewers (`!give`)
- Local SQLite database – no external server needed

---

### 🚀 Installation

1. **Download** – Grab the latest `.exe` from [Releases](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)
2. **Install** – Run the setup, done
3. **Configure** – Open the bot, enter channel + OAuth token, connect
4. **OBS** – Add browser source with `http://localhost:8765/` (1920×1080)

Get your OAuth token at [twitchtokengenerator.com](https://twitchtokengenerator.com/).

---

### 📋 Chat Commands

| Command | Description |
|---|---|
| `!raub <bet>` | Start or join a bank heist |
| `!ticket <amount>` | Buy raffle tickets |
| `!coins` | Check balance |
| `!topliste` | Top 5 robbers |
| `!top` | Top 10 (mods only) |
| `!give @User <amount>` | Gift currency |
| `!heistbot` | Bot info & version |

---

### 💻 Tech Stack

| | |
|---|---|
| App | Electron |
| Twitch | tmi.js |
| Animations | Phaser 3 + GSAP |
| Database | SQLite (better-sqlite3) |
| Updates | electron-updater |

---

### 🗺️ Roadmap

- [x] Heist system with dynamic multipliers
- [x] Animated OBS overlay
- [x] Police surround & SWAT intervention
- [x] Raffle system with overlay animation
- [ ] Extended dashboard statistics
- [ ] Custom sound upload
- [ ] Additional overlay themes

---

### 🤝 Contribute & Support

- 🐛 Found a bug? → [Open an issue](https://github.com/Benjamin-Web/Heist_Bot_Updates/issues)
- 💬 Questions? → [Discord Server](https://discord.gg/FV83Fcu3V3)
- ☕ Support the project? → [Ko-fi](https://ko-fi.com/benjaminweb)

---

*Current version: v1.3.5*
