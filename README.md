# 🍄 Super Mario — DeepSeek & OMP_GLM-5.3 Editions

**English** | [Українська](README.UA.md) | [Русский](README.RU.md) | [Deutsch](README.DE.md) | [Français](README.FR.md) | [Português](README.PT.md)

Experimental Super Mario–style platformers packed into **single HTML files** and built with AI: the original **DeepSeek Edition** — in a chat with the **DeepSeek** AI; the extended **OMP_GLM-5.3 Edition** — with **GLM-5.3** (the omp coding assistant). No frameworks, no build step — just open a file in a browser and play.

> 🤖 **Experiment notice:** the entire original game (HTML + CSS + JavaScript, ~1,770 lines) was generated through a conversation with DeepSeek and then refined. The OMP_GLM-5.3 Edition was, in turn, written with the GLM-5.3 model (omp assistant). Both are published as examples of AI-assisted game development. The full DeepSeek chat log (`log.txt`) stays out of the repository.

## ▶️ How to Play

1. Download or clone this repository.
2. Open one of the two game files in any modern browser (Chrome, Firefox, Safari, Edge):
   — `SuperMarioDeepSeek.html` — the original experiment;
   — `SuperMarioOMP.html` — the extended OMP Edition (see "Game Variants").
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

## 📦 Game Variants

| File | Description |
|---|---|
| `SuperMarioDeepSeek.html` | **DeepSeek Edition** — the original experiment: one generated run, bonuses, lives, top-10 leaderboard. |
| `SuperMarioOMP.html` | **OMP_GLM-5.3 Edition** — 3 themed levels (green hills → sunset desert → snowy night), stompable goomba enemies, coins, power-ups (⭐ invincibility star, 🍄 extra-life mushroom, 🧲 bonus magnet), springs, moving platforms, a ×2…×5 combo multiplier, sounds and chiptune music (Web Audio), parallax backgrounds, particles and screen shake. Keeps its own leaderboard. |

More variants of the game are still planned.

## ⚖️ License

Released under the [MIT License](LICENSE) — free to use, copy, modify, and redistribute.

**Disclaimer:** this is a non-commercial fan-made project and is not affiliated with or endorsed by Nintendo. All Mario-related trademarks belong to their respective owners.
