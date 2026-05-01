# 🦹‍♂️ Heist Bot - Der ultimative Twitch-Raubzug!

[Deutsch](#deutsch) | [English](#english)

---

<a name="deutsch"></a>
# Deutsch

Ein professioneller Twitch-Bot für Streamer, der Interaktion durch spannende Minispiele fördert. Mit Banküberfall-System, Raffle-Verlosungen, animiertem OBS-Overlay, Statistik-Dashboard und automatischen Updates – alles in einer Electron-App.

---

## ✨ Features

### 🎮 Heist-System
- Zuschauer starten mit `!raub <Einsatz>` einen Banküberfall oder schließen sich an
- Je mehr Leute mitmachen, desto höher der Multiplikator – aber auch das Risiko
- Polizei-Umzingelung bei Niederlage, SEK-Einsatz inklusive
- 60 Sekunden Joining-Phase mit animierten Räuber-Charakteren im Overlay
- **🧟 Zombie-Hunde Modus:** Alternativer Spielmodus (Wurstfabrik-Thema) als PRO Feature

### 🎫 Raffle-System
- Verlosungen direkt aus dem Dashboard starten
- Zuschauer kaufen mit `!ticket <Anzahl>` Lose
- Animierte Gewinnziehung im Overlay mit Claim-Mechanik (30 Sek. Timeout)
- Einstellbar: Ticket-Preis, Max-Tickets pro User
- **Sub-Only Modus** mit optionaler Mindest-Abo-Dauer
- Redraw-Option falls Gewinner nicht reagiert

### 🖥️ OBS Overlay
- Animierter Räuber-Lauf am unteren Bildschirmrand (22 verschiedene Skins!)
- Bank-Gebäude, Sirenen, Soundeffekte
- Konfetti bei Raffle-Gewinn, Polizei-Animation bei Heist-Niederlage
- Sauber transparent für OBS – einfach als Browser-Quelle einbinden

### 📊 Statistik-Dashboard
- Heist-Statistiken: Gesamtzahl, Winrate, Ø Teilnehmer, Gesamteinsatz, Gewinn/Verlust
- Raffle-Statistiken: Gesamtzahl, Claim-Quote, verteilte Preise
- Winrate-Trend als Balkendiagramm (filterbar: 7/14/30/90 Tage oder Gesamtzeit)
- Letzte Heists & Raffles im Überblick
- Detaillierte Viewer-Statistiken

### 📋 Dashboard
- Alles auf einen Blick: Heist-Status, Leaderboard, Event-Log
- Manuelle Währungsverteilung an einzelne Nutzer oder alle
- Spiel-Einstellungen: Währungsname, Watch-Time-Belohnung, Sub-Boni (Tier 1/2/3)
- Auto-Updates direkt in der App

### 🌍 Mehrsprachigkeit
- **5 Sprachen:** Deutsch, English, 中文 (Chinesisch), Español, Русский
- Sprache im Dashboard mit einem Klick umschaltbar
- OBS-Overlay passt sich automatisch an

### ⭐ PRO Features
- **Custom Commands:** Erstelle eigene Bot-Befehle (!ad, !discord, !sound, etc.)
- **Excluded Accounts:** Schließe Bots/Accounts aus der Topliste aus
- **Erweiterte Statistiken:** Detaillierte Heist- und Raffle-Analysen
- **Zombie-Hunde Modus:** Alternativer Spielmodus
- Aktivierung über Ko-fi mit euren Twitch: [Namen]

### 💰 Währung & Treue
- Automatische Watch-Time-Belohnung (alle 5 Min)
- Sub-Boni für Tier 1, 2 und 3
- Schenkfunktion zwischen Zuschauern (`!give`)
- Lokale SQLite-Datenbank – kein externer Server nötig

### 🚀 Weitere Features
- **Auto-Updates:** Der Bot prüft beim Start automatisch auf neue Versionen
- **Login-System:** E-Mail-basierte Registrierung für PRO-Features
- **💾 Lokale Datenbank:** Alle Spielerdaten bleiben sicher auf deinem PC

---

## 🚀 Installation & Setup

1. **Herunterladen:** Lade die neueste `HeistBot-Setup-x.x.x.exe` von der **[Releases-Seite](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)** herunter.
2. **Installieren:** Führe die `.exe` aus und folge den Anweisungen.
3. **Konfigurieren:** Starte den Bot, gib deinen Kanal und dein Token ein und klicke auf "Verbinden". ✨

### OBS Overlay hinzufügen
1. Erstelle eine neue **Browser-Quelle** in OBS.
2. URL: `http://localhost:8765/?lang=de` (Standard-Port)
3. Breite: `1920`, Höhe: `1080`
4. Aktiviere "Audio über OBS steuern", falls gewünscht.

OAuth-Token bekommst du auf [twitchtokengenerator.com](https://twitchtokengenerator.com/).

---

## 🎮 Chat-Befehle

| Befehl | Beschreibung |
|--------|-------------|
| `!raub <Einsatz>` / `!heist <Bet>` | Startet einen Banküberfall oder tritt einem bei |
| `!ticket <Anzahl>` / `!raffle` / `!lose` | Kauft Lose für die aktuelle Verlosung |
| `!coins` / `!münzen` / `!<Währungsname>` | Zeigt den aktuellen Kontostand |
| `!topliste` / `!leaderboard` | Zeigt die Top 5 Räuber |
| `!top` | (Mod/Broadcaster) Zeigt die Top 10 |
| `!give @User <Betrag>` / `!schenken` | Verschenke Währung an andere |
| `!heistbot` / `!raubbot` / `!botinfo` | Zeigt Bot-Version |

---

## 💻 Tech Stack

- **Framework:** Electron
- **Twitch API:** tmi.js
- **Grafik/Physik:** Phaser 3 & GSAP
- **Datenbank:** SQLite (lokal) + Supabase (PRO Backend)
- **Backend:** Express.js (PRO Features)

---

## 🗺️ Roadmap

- [x] 🎮 Heist-System mit dynamischen Multiplikatoren
- [x] 🖥️ Animiertes OBS-Overlay (22 Skins)
- [x] 🚨 Polizei-Umzingelung & SEK-Einsatz
- [x] 🎫 Raffle-System mit Overlay-Animation
- [x] 📊 Erweiterte Statistiken im Dashboard
- [x] 🌍 5 Sprachen (DE, EN, ZH, ES, RU)
- [x] ⭐ PRO Features (Custom Commands, Excluded Accounts)
- [x] 🧟 Zombie-Hunde Spielmodus
- [ ] 🔊 Custom Sound-Upload
- [ ] 🎨 Weitere Overlay-Themes

---

## 🤝 Mitmachen & Support

- 🐛 Bug gefunden? → [Issue erstellen](https://github.com/Benjamin-Web/Heist_Bot_Updates/issues)
- 💬 Fragen? → [Discord Server](https://discord.gg/FV83Fcu3V3)
- ☕ Unterstützen? → [Ko-fi](https://ko-fi.com/ronincannons)

## 📄 Lizenz

Dieses Projekt ist lizenziert unter der ISC Lizenz.

Aktuell: **v1.3.7**

---

*Entwickelt mit ❤️ für die Twitch-Community.*

---

<a name="english"></a>
# English

A professional Twitch bot for streamers that promotes interaction through exciting mini-games. With a bank robbery system, raffle giveaways, animated OBS overlay, statistics dashboard, and automatic updates – all in one Electron app.

---

## ✨ Features

### 🎮 Heist System
- Viewers start a bank heist with `!raub <bet>` or join one in progress
- More participants = higher multiplier, but also higher risk
- Police surround animation on loss, SWAT intervention included
- 60-second joining phase with animated robber characters in the overlay
- **🧟 Zombie Dog Mode:** Alternative game mode (sausage factory theme) as PRO feature

### 🎫 Raffle System
- Start giveaways directly from the dashboard
- Viewers buy tickets with `!ticket <amount>`
- Animated winner draw in the overlay with claim mechanic (30 sec timeout)
- Configurable: ticket price, max tickets per user
- **Sub-Only Mode** with optional minimum subscription duration
- Redraw option if the winner doesn't respond

### 🖥️ OBS Overlay
- Animated robber parade at the bottom of the screen (22 different skins!)
- Bank building, sirens, sound effects
- Confetti on raffle win, police animation on heist loss
- Clean transparent background for OBS – just add as browser source

### 📊 Statistics Dashboard
- Heist statistics: total count, win rate, avg. participants, total wagered, profit/loss
- Raffle statistics: total count, claim rate, distributed prizes
- Win rate trend as bar chart (filterable: 7/14/30/90 days or all-time)
- Recent heists & raffles at a glance
- Detailed viewer statistics

### 📋 Dashboard
- Everything at a glance: heist status, leaderboard, event log
- Manual currency distribution to individual users or everyone
- Game settings: currency name, watch-time reward, sub bonuses (Tier 1/2/3)
- Auto-updates built right in

### 🌍 Multi-Language
- **5 Languages:** Deutsch, English, 中文 (Chinese), Español, Русский
- Switch language in the dashboard with one click
- OBS overlay adapts automatically

### ⭐ PRO Features
- **Custom Commands:** Create your own bot commands (!ad, !discord, !sound, etc.)
- **Excluded Accounts:** Exclude bots/accounts from the leaderboard
- **Extended Statistics:** Detailed heist and raffle analysis
- **Zombie Dog Mode:** Alternative game mode
- Activation via Ko-fi with your Twitch: [Name]

### 💰 Currency & Loyalty
- Automatic watch-time rewards (every 5 min)
- Sub bonuses for Tier 1, 2, and 3
- Gift system between viewers (`!give`)
- Local SQLite database – no external server needed

### 🚀 More Features
- **Auto-Updates:** The bot automatically checks for new versions at startup
- **Login System:** Email-based registration for PRO features
- **💾 Local Database:** All player data stays safe on your PC

---

## 🚀 Installation & Setup

1. **Download:** Grab the latest `HeistBot-Setup-x.x.x.exe` from the **[Releases Page](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)**.
2. **Install:** Run the `.exe` and follow the instructions.
3. **Configure:** Start the bot, enter your channel and token, and click "Connect". ✨

### Add OBS Overlay
1. Create a new **Browser Source** in OBS.
2. URL: `http://localhost:8765/?lang=en` (Default Port)
3. Width: `1920`, Height: `1080`
4. Enable "Control audio via OBS" if desired.

Get your OAuth token at [twitchtokengenerator.com](https://twitchtokengenerator.com/).

---

## 🎮 Chat Commands

| Command | Description |
|---------|-------------|
| `!raub <bet>` / `!heist <bet>` | Start a bank heist or join one |
| `!ticket <amount>` / `!raffle` / `!lose` | Buy tickets for the current raffle |
| `!coins` / `!<currency name>` | Show current balance |
| `!topliste` / `!leaderboard` | Show top 5 robbers |
| `!top` | (Mod/Broadcaster) Show top 10 |
| `!give @User <amount>` | Gift currency to others |
| `!heistbot` / `!botinfo` | Show bot version |

---

## 💻 Tech Stack

- **Framework:** Electron
- **Twitch API:** tmi.js
- **Graphics/Physics:** Phaser 3 & GSAP
- **Database:** SQLite (local) + Supabase (PRO backend)
- **Backend:** Express.js (PRO features)

---

## 🗺️ Roadmap

- [x] 🎮 Heist system with dynamic multipliers
- [x] 🖥️ Animated OBS overlay (22 skins)
- [x] 🚨 Police surround & SWAT intervention
- [x] 🎫 Raffle system with overlay animation
- [x] 📊 Extended dashboard statistics
- [x] 🌍 5 Languages (DE, EN, ZH, ES, RU)
- [x] ⭐ PRO features (custom commands, excluded accounts)
- [x] 🧟 Zombie dog game mode
- [ ] 🔊 Custom sound upload
- [ ] 🎨 Additional overlay themes

---

## 🤝 Contribute & Support

- 🐛 Found a bug? → [Open an issue](https://github.com/Benjamin-Web/Heist_Bot_Updates/issues)
- 💬 Questions? → [Discord Server](https://discord.gg/FV83Fcu3V3)
- ☕ Support the project? → [Ko-fi](https://ko-fi.com/ronincannons)

## 📄 License

This project is licensed under the ISC License.

Current version: **v1.3.7**

---

*Developed with ❤️ for the Twitch community.*
