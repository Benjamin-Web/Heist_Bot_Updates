# 🦹‍♂️ Heist Bot - Der ultimative Twitch-Raubzug!

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
3. Breite: `1920`, Höhe: `1080`
4. Aktiviere "Audio über OBS steuern", falls gewünscht.

---

## 🎮 Zuschauer-Befehle

- `!raub <einsatz>` - Startet einen Banküberfall oder nimmt an einem bestehenden teil.
- `!coins` (oder dein Währungsname) - Zeigt den aktuellen Kontostand an.
- `!topliste` - Zeigt die Top 5 Räuber im Chat an.
- `!top` - (Mod/Broadcaster) Zeigt die Top 10 Bestenliste an.
- `!heistbot` - Zeigt Informationen zur aktuellen Bot-Version.

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

*Entwickelt mit ❤️ für die Twitch-Community.*
