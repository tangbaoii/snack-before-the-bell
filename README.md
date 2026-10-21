# Snack Before the Bell: How to Play

**One line:** You skipped breakfast. Eat every snack on your desk before the bell rings, and don't let the teacher catch you.

## Running it
Open `index.html` in Chrome or Edge. It needs an internet connection to load three.js. All models are built in code and all sounds are generated in the browser, so there are no asset files.

## Controls
| Key | Action |
|---|---|
| `←` / `→`, `Q` / `E`, or click a snack | Switch snacks |
| `W` `A` `S` `D` | Type the sequence shown above the snack |
| `Esc` | Pause |
| `Enter` / `R` on result screen | Continue / Retry |

## Rules
1. Five snacks sit on your desk. In later classes, refills come out of your bag (the HUD shows "Bag"). Eat every snack to clear the class.
2. The first correct key **locks** you onto a snack. You must finish it or spit it out before switching.
3. **Wrong key**: you spit it out. Progress resets and input freezes for 3 seconds (a green tint and a draining bar, no countdown).
4. **Teacher turns around**: pressing ANY key, even while frozen, gets you caught and you lose.
5. Warning signs before a turn: the chalk stops, footsteps plus a beep (sometimes a cough), the teacher twists and glances over his shoulder, a ❓ appears over his head, the HUD shows "⚠️ Turning…", and a yellow banner appears. While the teacher watches: a red "👀 FREEZE!" banner, a pulsing red border, and an alarm sound. Nervous classmates looking back 💦 are an extra hint. **Fake-outs:** from Class 2 on, the teacher sometimes shows all the warning signs and then goes back to writing.
6. Clear the desk before the bell to win. Stars: 1 for clearing, 2 for 20%+ of the time left, 3 for 40%+ left.

| Class | Snacks | Time | Turn every | Fake-out chance |
|---|---|---|---|---|
| 1 Math | 5 | 90s | 5–9s | 0% |
| 2 Literature | 6 | 90s | 4.5–8s | 20% |
| 3 English | 7 | 90s | 4–7.5s | 25% |
| 4 Physics | 8 | 85s | 3.5–7s | 30% |
| 5 History | 9 | 85s | 3–6s | 35% |

| Snack | Points | Keys |
|---|---|---|
| Bun | 10 | 4 |
| Energy Jelly | 15 | 5 |
| Onigiri | 20 | 6 |
| Sandwich | 40 | 8 |
| Noodle Hot Dog | 55 | 9 |
| Fried Chicken | 70 | 10 |
| Bubble Tea | 100 | 12 |

## Tuning
Edit `LEVELS` and `FOODS` at the top of the script in `index.html`: time, turn interval `turnEvery`, watch duration `watch`, warning length `warn`, fake-out chance `fake`, the snack list `items`, and sequence lengths.
