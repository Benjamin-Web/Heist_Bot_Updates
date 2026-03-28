[Deutsch](#deutsch) | [English](#english)

---

<a name="deutsch"></a>
# Deutsch

Ein professioneller Twitch-Bot für Streamer, der Interaktion durch ein spannendes "Banküberfall"-Minispiel fördert. Mit integriertem Dashboard, Overlay-System und automatischen Updates.

---

## ✨ Features

- **🎮 Heist Minispiel:** Zuschauer können mit `!raub <bet>` gemeinsam Banken überfallen und fiktive Währung gewinnen.
- **🌍 Mehrsprachigkeit:** Volle Unterstützung für **Deutsch** und **Englisch**. Die Sprache lässt sich im Dashboard mit einem Klick umschalten.
- **✨ Dynamische Räuber-Parade:** Zuschauer erscheinen während der Joining-Phase als animierte Räuber-Charaktere im OBS Overlay, laufen am unteren Bildschirmrand entlang und interagieren mit verschiedenen Animationen.
- **📊 Live Dashboard:** Verwalte Kanaleinstellungen, OAuth-Token und Belohnungen in Echtzeit über eine moderne Oberfläche.
- **🖥️ OBS Overlay:** Integrierter WebSocket-Server für visuelle und akustische Benachrichtigungen im Stream (Intro, Sieg, Niederlage, SWAT-Einsatz).
- **💰 Treue-System:** Automatische Belohnungen für Zuseh-Zeit (Watch-Time) und Subs (Tier 1, 2 & 3).
- **🏆 Leaderboard:** Behalte den Überblick über die erfolgreichsten Räuber deines Kanals.
- **🚀 Auto-Updates:** Der Bot prüft beim Start automatisch auf neue Versionen und kann sich selbst aktualisieren.
- **💾 Lokale Datenbank:** Alle Daten werden effizient in einer lokalen SQLite-Datenbank gespeichert.

---

### Installation & Setup

1. **Herunterladen:** Lade die neueste `HeistBot-Setup-x.x.x.exe` von der **[Releases-Seite](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)** herunter.
2. **Installieren:** Führe die `.exe` aus und folge den Anweisungen.
3. **Konfigurieren:** Starte den Bot, gib deinen Kanal und dein Token ein und klicke auf "Verbinden". ✨

---

## 🛠️ Konfiguration

1. Starte den Bot und trage deinen **Kanalnamen** sowie dein **OAuth-Token** im Dashboard ein.
2. Definiere den Namen deiner **Währung** (z.B. "Batzen", "Coins", "Dukaten").
3. Stelle die Belohnungen für Watch-Time und Subs ein.
4. Klicke auf **Verbinden**, um den Bot live zu schalten.

### OBS Overlay hinzufügen
1. Erstelle eine neue **Browser-Quelle** in OBS.
2. URL: `http://localhost:8765/` (Standard-Port)
3. Breite: `1920`, Height: `1080`
4. Aktiviere "Audio über OBS steuern", falls gewünscht.

---

## 🎮 Zuschauer-Befehle

- `!raub <einsatz>` / `!heist <bet>` - Startet einen Banküberfall oder nimmt an einem bestehenden teil.
- `!coins` / `!münzen` (oder dein Währungsname) - Zeigt den aktuellen Kontostand an.
- `!topliste` / `!leaderboard` - Zeigt die Top 5 Räuber im Chat an.
- `!top` - (Mod/Broadcaster) Zeigt die Top 10 Bestenliste an.
- `!give @User <Amount>` / `!schenken @Nutzer <Betrag>` - Verschenke deine Währung an andere.
- `!heistbot` / `!raubbot` - Zeigt Informationen zur aktuellen Bot-Version.

---

## 💻 Tech Stack

- **Framework:** Electron
- **Twitch API:** tmi.js
- **Grafik/Physik:** Phaser 3 & GSAP
- **Datenbank:** SQLite

---

## 📄 Lizenz

Dieses Projekt lizenziert unter der ISC Lizenz.

---

## 🛠️ Roadmap (Geplante Features)

- [ ] **🎫 Neues Raffle-System:** Ein faires und spannendes Gewinnspiel-System für deine Zuschauer.
- [ ] **✨ Erweiterte Heist-Effekte:** Noch packendere Animationen und Soundeffekte für den Banküberfall.
- [ ] **📊 Erweiterte Statistiken:** Detaillierte Auswertungen der erfolgreichsten Heists im Dashboard.

---

*Entwickelt mit ❤️ für die Twitch-Community.*

---

<a name="english"></a>
# English

A professional Twitch bot for streamers that promotes interaction through an exciting "bank robbery" mini-game. With integrated dashboard, overlay system, and automatic updates.

---

## ✨ Features

- **🎮 Heist Minigame:** Viewers can rob banks together with `!raub <bet>` and win fictional currency.
- **🌍 Multi-language:** Full support for **German** and **English**. The language can be toggled in the dashboard with one click.
- **✨ Dynamic Robber Parade:** Viewers appear as animated robber characters in the OBS overlay during the joining phase, walking along the bottom of the screen and interacting with various animations.
- **📊 Live Dashboard:** Manage channel settings, OAuth tokens, and rewards in real-time through a modern interface.
- **🖥️ OBS Overlay:** Integrated WebSocket server for visual and acoustic notifications in the stream (intro, victory, defeat, SWAT intervention).
- **💰 Loyalty System:** Automatic rewards for watch time and subs (Tier 1, 2 & 3).
- **🏆 Leaderboard:** Keep track of the most successful robbers on your channel.
- **🚀 Auto-Updates:** The bot automatically checks for new versions at startup and can update itself.
- **💾 Local Database:** All data is efficiently stored in a local SQLite database.

---

### Installation & Setup

1. **Download:** Download the latest `HeistBot-Setup-x.x.x.exe` from the **[Releases Page](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)**.
2. **Install:** Run the `.exe` and follow the instructions.
3. **Configure:** Start the bot, enter your channel and token, and click "Connect". ✨

---

## 🛠️ Configuration

1. Start the bot and enter your **channel name** and **OAuth token** in the dashboard.
2. Define the name of your **currency** (e.g., "Batzen", "Coins", "Doubloons").
3. Set rewards for watch time and subs.
4. Click **Connect** to take the bot live.

### Add OBS Overlay
1. Create a new **Browser Source** in OBS.
2. URL: `http://localhost:8765/` (Default Port)
3. Width: `1920`, Height: `1080`
4. Enable "Control audio via OBS" if desired.

---

## 🎮 Viewer Commands

- `!raub <bet>` - Starts a bank robbery or joins an existing one.
- `!coins` (or your currency name) - Shows the current balance.
- `!topliste` - Shows the top 5 robbers in chat.
- `!top` - (Mod/Broadcaster) Shows the top 10 leaderboard.
- `!heistbot` - Shows information about the current bot version.

---

## 💻 Tech Stack

- **Framework:** Electron
- **Twitch API:** tmi.js
- **Graphics/Physics:** Phaser 3 & GSAP
- **Database:** SQLite

---

## 📄 License

This project is licensed under the ISC License.

---

## 🛠️ Roadmap (Planned Features)

- [ ] **🎫 New Raffle System:** A fair and exciting giveaway system for your viewers.
- [ ] **✨ Enhanced Heist Effects:** Even more gripping animations and sound effects for the bank robbery.
- [ ] **📊 Advanced Statistics:** Detailed analysis of the most successful heists in the dashboard.

---

*Developed with ❤️ for the Twitch community.*

