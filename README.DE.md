# 🍄 Super Mario — DeepSeek Edition

[English](README.md) | [Українська](README.UA.md) | [Русский](README.RU.md) | **Deutsch** | [Français](README.FR.md) | [Português](README.PT.md)

Ein experimentelles Jump-’n’-Run im Stil von Super Mario, gepackt in **eine einzige HTML-Datei**, gemeinsam mit dem **DeepSeek**-KI-Chat erstellt. Keine Frameworks, kein Build-Schritt — einfach die Datei im Browser öffnen und losspielen.

> 🤖 **Hinweis zum Experiment:** Das gesamte Spiel (HTML + CSS + JavaScript, ca. 1.770 Zeilen) wurde in einem Dialog mit DeepSeek generiert und anschließend verfeinert. Es wird als Beispiel für KI-gestützte Spieleentwicklung veröffentlicht. Das vollständige Chat-Protokoll (`log.txt`) bleibt außerhalb des Repositorys.

## ▶️ So spielen Sie

1. Laden Sie dieses Repository herunter oder klonen Sie es.
2. Öffnen Sie eine der beiden Spieldateien in einem modernen Browser (Chrome, Firefox, Safari, Edge):
   — `SuperMarioDeepSeek.html` — das originale Experiment;
   — `SuperMarioOMP.html` — die erweiterte OMP Edition (siehe „Spielvarianten“).
3. Geben Sie Ihren Spielernamen ein — und los!

Kein Server, keine Installation, keine Abhängigkeiten.

## 🎮 Steuerung

| Aktion | Tastatur | Bildschirm-Button |
|---|---|---|
| Start / Pause | `Leertaste` | ▶ Start / Pause |
| Nach links | `←` | ◀ Links |
| Nach rechts | `→` | Rechts ▶ |
| Springen | `↑` | ⤒ Springen |
| Ducken (unter Hindernissen durchrutschen) | `↓` | ⤓ Ducken |
| Neustart des Laufs | `Esc` | ⟲ Neustart |

Die Bewegung erfolgt mit Trägheit: Mario beschleunigt, solange man eine Richtung hält, und bremst zuerst beim Richtungswechsel — das klassische Spielgefühl.

## 🕹️ Gameplay

- Die Strecke mit Hindernissen, Gruben und Boni wird zu Beginn jedes Laufs generiert.
- Sammeln Sie Boni: 🍒 Kirsche — **1 Punkt**, 🍎 Apfel — **2 Punkte**, 🍯 Honig — **3 Punkte**.
- Einen Bonus verpasst? Sie können umkehren und ihn doch noch holen.
- Ein Sturz in eine Grube kostet **1 von 3 Leben** ❤❤❤ — der Lauf startet neu. Alle drei verloren, beginnt das Spiel von vorn.
- Erreichen Sie das Ziel, erhalten Sie einen Bonus von **10 Punkten × verbleibende Leben**.

## 🏆 Bestenliste und Verlauf

- Der aktuelle Punktestand wird über der Bestenliste angezeigt.
- Die **Top-10-Bestenliste** bleibt sortiert, höchster Punktestand oben (Platz, Name, Bestleistung).
- Übertrifft Ihr Punktestand die Liste, fliegt der unterste Eintrag heraus.
- Die **letzten 10 Spiele** werden in einer separaten Liste angezeigt.
- Alles wird im `localStorage` des Browsers gespeichert — Ihr Verlauf ist beim nächsten Mal noch da.

> Hinweis: Die Spielsprache der Benutzeroberfläche ist Russisch.

## 🛠️ Technik

- Eine eigenständige Datei: HTML + CSS + JavaScript.
- Darstellung auf einem HTML5-`<canvas>` (900 × 400).
- Speicherung über `localStorage`.
- Bonus-Sprites werden programmatisch gezeichnet — keine Bilddateien.

## 📦 Spielvarianten

| Datei | Beschreibung |
|---|---|
| `SuperMarioDeepSeek.html` | Das originale Experiment: ein generierter Lauf, Boni, Leben, Top-10-Bestenliste. |
| `SuperMarioOMP.html` | **OMP Edition** — 3 Level mit Themen (grüne Hügel → Sonnenuntergangs-Wüste → verschneite Nacht), bespringbare Gumba-Gegner, Münzen, Power-Ups (⭐ Unverwundbarkeitsstern, 🍄 Extra-Leben-Pilz, 🧲 Bonus-Magnet), Sprungfedern, bewegliche Plattformen, ×2…×5-Kombo-Multiplikator, Sounds und Chiptune-Musik (Web Audio), Parallax-Hintergründe, Partikel und Bildschirmwackeln. Eigene Bestenliste. |

Weitere Spielvarianten sind weiter geplant.

## ⚖️ Lizenz

Veröffentlicht unter der [MIT-Lizenz](LICENSE) — kostenlose Nutzung, Vervielfältigung, Änderung und Weitergabe.

**Haftungsausschluss:** Dies ist ein nichtkommerzielles Fanprojekt und steht in keiner Verbindung zu Nintendo. Alle Marken im Zusammenhang mit Mario gehören ihren jeweiligen Eigentümern.
