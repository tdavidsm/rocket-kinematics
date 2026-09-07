# 🚀 Rocket Kinematics — Beat the Bots

A browser-based kinematics game: three challenges, one for each acceleration equation. Students choose their rocket's launch settings, **do the physics**, and race two computer opponents. Runs entirely in the browser — no install, no accounts.

**▶ Play:** https://tdavidsm.github.io/rocket-kinematics/

## The three challenges

| # | Name | Equation | Given | You pick |
|---|------|----------|-------|----------|
| 1 | **Timed Burn** | `vf = vi + a·t` | burn time & target final speed | vᵢ, a |
| 2 | **Speed Gate** | `vf² = vi² + 2·a·d` | gate distance & target speed at the gate | vᵢ, a |
| 3 | **Target Landing** | `d = vi·t + ½·a·t²` | flight time & target distance | vᵢ, a |

Each equation has **two unknowns and one relationship**, so students *choose* one value (say vᵢ) and **calculate** the other (a) to hit the target — real equation-rearranging, three different ways.

## How it plays
- **🧪 Test flight** — fly your rocket alone and see your result; every test is saved to a flight log so students can *gather data* and refine.
- **🚀 Race the bots** — run against two computer rockets. **Closest to the target wins.** Beat *both* to clear the challenge and earn its ★.
- The bots are each set to a **random 75–90% of optimal** every race — good, but beatable if your math is sharp. A student who computes correctly gets essentially zero error and wins; a guesser loses to the smarter bot.

## Teaching notes
- **Numbers are randomized** (🎲 New numbers) so each student/period gets different values — no answer-sharing. Every challenge always has a near-exact solution on the allowed grid.
- After each run the app shows the **worked substitution** (e.g. `vf = 5.0 + 5.0×4.0 = 25.00 m/s`) for instant feedback and debrief.
- **Rules:** acceleration is always forward and **≥ 0.5 m/s²** (steps of **0.1**); initial velocity moves in steps of **0.5 m/s**.
- Built touch-first for **iPad Safari** — big steppers, no hover or keyboard needed.

## Tech
Single self-contained `index.html` — plain HTML/CSS/JS, canvas rocket animation (starfield, gate/target markers, live speed readouts), no dependencies. Deployed via GitHub Pages from `main`.
