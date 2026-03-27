# 🦹‍♂️ Heist Bot - Der ultimative Twitch-Raubzug!

Moin! Ich hab hier mal was zusammengebastelt, weil ich Bock auf ein interaktives Heist-Game für Twitch hatte. Hat mich echt einige Nächte gekostet, aber ich find's jetzt eigentlich ziemlich cool.

---

## ✨ Was kann der Bot?

- **🎮 Banküberfall-Minispiel:** Mit `!raub <einsatz>` können Zuschauer zusammenarbeiten, um virtuelles Geld zu erbeuten.
- **🌍 Zweisprachig:** Komplett auf Deutsch und Englisch verfügbar (einfach im Dashboard umschalten).
- **✨ Animierte Räuber im Stream:** Wer beim Heist mitmacht, taucht als kleiner, animierter Charakter im OBS-Overlay auf und läuft durchs Bild.
- **📊 Dashboard:** Eine leichte Benutzeroberfläche, um den Bot, deine Währung und Belohnungen schnell einzustellen.
- **🖥️ OBS-Overlay:** Bringt Sounds und Animationen direkt in deinen Stream (inklusive SWAT-Alarm, Siege oder Fails).
- **💰 Belohnungssystem:** Vergib ganz automatisch Coins fürs Zuschauen (Watch-Time) oder für Subs.
- **🏆 Toplisten:** Finde heraus, wer im Chat am meisten abgestaubt hat.
- **🚀 Auto-Updates:** Der Bot checkt beim Start von selbst, ob es eine neue Version gibt.
- **💾 Lokale Speicherung:** Alle Daten (wie der Kontostand der User) bleiben rein lokal bei dir auf dem Rechner in einer SQLite-Datenbank.

---

## 🚀 Installation & Setup

1. **Download:** Hol dir die aktuellste `HeistBot-Setup-x.x.x.exe` von den **[Releases](https://github.com/Benjamin-Web/Heist_Bot_Updates/releases)**.
2. **Installieren:** Einfach ausführen und den Anweisungen folgen.
3. **Start:** Bot öffnen, Twitch-Kanal und OAuth-Token eintragen, fertig!

---

## 🛠️ Einrichten

1. Starte den Bot und trage im Dashboard deinen **Kanalnamen** und das **OAuth-Token** ein.
2. Denk dir einen Namen für deine **Währung** aus (z.B. "Batzen", "Coins", "Dukaten").
3. Stell ein, wie viele Coins Zuschauer für Watch-Time und Subs bekommen sollen.
4. Klick auf **Verbinden**, um loszulegen.

### OBS-Overlay hinzufügen
1. Erstelle in OBS eine neue **Browser-Quelle**.
2. URL: `http://localhost:8765/` (das ist der Standard-Port)
3. Breite: `1920`, Höhe: `1080`
4. Setze den Haken bei "Audio über OBS steuern", wenn du die Lautstärke direkt in OBS regeln willst.

---

## 💬 Chat-Befehle

- `!raub <einsatz>` / `!heist <bet>` – Startet einen Heist oder tritt einem bei.
- `!coins` / `!münzen` (oder dein eigener Währungsname) – Zeigt den aktuellen Kontostand des Users an.
- `!topliste` / `!leaderboard` – Zeigt die Top 5 der reichsten Räuber im Chat.
- `!top` – (Für Mods/Streamer) Spuckt die Top 10 Bestenliste im Chat aus.
- `!give @User <Menge>` / `!schenken @Nutzer <Menge>` – Geld an andere im Chat verschenken.
- `!heistbot` / `!raubbot` – Zeigt Infos zur aktuellen Version des Bots.

---

## 💻 Tech Stack

Falls es dich interessiert, was unter der Haube steckt:
- **Framework:** Electron
- **Twitch API:** tmi.js
- **Grafik/Physik im Overlay:** Phaser 3 & GSAP
- **Datenbank:** SQLite

---

## 📄 Lizenz

Dieses Projekt steht unter der ISC Lizenz.

---

## 📅 Roadmap (Geplante Features)

- [ ] **🎫 Raffle-System:** Ein Gewinnspiel-System für den Chat.
- [ ] **✨ Mehr Heist-Effekte:** Noch detailliertere Animationen und Sounds während des Überfalls.
- [ ] **📊 Bessere Statistiken:** Auswertungen der erfolgreichsten Raubzüge direkt im Dashboard.

---
Ist alles noch ein bisschen "Work in Progress", aber ich find's echt stabil bisher. Falls ihr Bugs findet oder Ideen habt, haut einfach raus. Viel Spaß beim Rauben! 💰✨

*Entwickelt mit ❤️ für die Twitch-Community.*
