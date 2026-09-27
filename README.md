# 🍄 Super Mario — DeepSeek Edition

**English** | [Українська](README.UA.md) | [Русский](README.RU.md) | [Deutsch](README.DE.md) | [Français](README.FR.md) | [Português](README.PT.md)

An experimental Super Mario–style platformer packed into a **single HTML file**, created together with the **DeepSeek** AI chat. No frameworks, no build step — just open the file in a browser and play.

> 🤖 **Experiment notice:** the entire game (HTML + CSS + JavaScript, ~1,770 lines) was generated through a conversation with DeepSeek and then refined. It is published as an example of AI-assisted game development. The full chat log (`log.txt`) stays out of the repository.

## ▶️ How to Play

1. Download or clone this repository.
2. Open `SuperMarioDeepSeek.html` in any modern browser (Chrome, Firefox, Safari, Edge).
3. Enter your player name — and go!

No server, no installation, no dependencies.

## 🎮 Controls

| Action | Keyboard | On-screen button |
|---|---|---|
| Start / Pause | `Space` | ▶ Start / Pause |
| Move left | `←` | ◀ Left |
| Move right | `→` | Right ▶ |
| Jump | `↑` | ⤒ Jump |
| Duck (slide under obstacles) | `↓` | ⤓ Duck |
| Restart the run | `Esc` | ⟲ Restart |

Movement is inertia-based: Mario accelerates while you hold a direction, brakes first when you reverse — just like the classic feel.

## 🕹️ Gameplay

- The route with obstacles, pits and bonuses is generated at the start of each run.
- Collect bonuses: 🍒 cherry — **1 pt**, 🍎 apple — **2 pts**, 🍯 honey — **3 pts**.
- Missed a bonus? You can turn back and grab it.
- Falling into a pit costs **1 of 3 lives** ❤❤❤ — the run restarts. Lose all three and the game starts over.
- Reach the finish and you earn a bonus of **10 pts × remaining lives**.

## 🏆 Score Table & History

- The current score is shown above the leaderboard.
- The **top-10 leaderboard** is kept sorted, highest score first (rank, name, best score).
- When your score beats the table, the lowest entry is pushed out.
- The **last 10 games** are listed separately.
- Everything is saved in the browser's `localStorage`, so your history is still there next time.

> Note: the in-game interface language is Russian.

## 🛠️ Tech

- One self-contained file: HTML + CSS + JavaScript.
- Rendering on an HTML5 `<canvas>` (900 × 400).
- Persistence via `localStorage`.
- Bonus sprites are drawn programmatically — no image assets.

## 🗺️ Roadmap

This is the first experiment. The plan is to try creating **a couple more variants** of the game based on this codebase.

## ⚖️ License

Released under the [MIT License](LICENSE) — free to use, copy, modify, and redistribute.

**Disclaimer:** this is a non-commercial fan-made project and is not affiliated with or endorsed by Nintendo. All Mario-related trademarks belong to their respective owners.
