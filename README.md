# Chew & Hide: How to Play

**One line:** You skipped breakfast. Eat every snack on your desk before the bell rings, and don't let the teacher catch you.

## ▶ Play now
**https://tangbaoii.github.io/snack-before-the-bell/**

## Running it
Open `index.html` in Chrome or Edge (needs internet to load three.js), or use `ChewAndHide.html`, a single file that works offline. All models are built in code and all sounds are generated in the browser, so there are no asset files.

## Controls
| Key | Action |
|---|---|
| `←` / `→`, `Q` / `E`, or click a snack | Switch snacks (the selected one glows, bounces, and has a ▼ pointer) |
| `W` `A` `S` `D` | Type the sequence shown above the snack |
| `Esc` | Pause |
| `Enter` / `R` on result screen | Continue / Retry |

## Rules
1. Five snacks sit on your desk. In later classes, refills come out of your bag (the HUD shows "Bag"). Eat every snack to clear the class.
2. The first correct key **locks** you onto a snack. You must finish it or spit it out before switching.
3. **Wrong key**: you spit it out. Progress resets and input freezes for 3 seconds (a green tint and a draining bar, no countdown).
4. **Teacher turns around**: pressing ANY key, even while frozen, gets you caught and you lose.
5. Warning signs before a turn: the chalk stops, footsteps plus a beep (sometimes a cough), the teacher twists and glances over his shoulder, a ❓ appears over his head, the HUD shows "⚠️ Turning…", and a yellow banner appears. The turn itself is slow in early classes. You're only caught once he's more than halfway around, and the turn speeds up in later classes. While the teacher watches: a red "👀 FREEZE!" banner, a pulsing red border, and an alarm sound. Nervous classmates looking back 💦 are an extra hint. **Fake-outs:** from Class 2 on, the teacher sometimes shows all the warning signs and then goes back to writing. He also sometimes turns **sideways to sip water** 🥤 (status shows "Drinking"). That one is safe.
6. **Varied looks:** some turns are quick glances (~1 s), some are long stares. After a long stare he gives you a bit more time before the next one.
7. **Sneaky deskmate (Class 3+):** if you stop in the middle of a snack for over ~2 seconds, your deskmate's hand creeps over 😋. Keep eating to scare it off. Otherwise he steals the half-eaten snack and a fresh one goes back into your bag. No extra controls needed.
8. **Surprise events (Classes 4–5):** a 📢 PA announcement makes everyone, including the teacher, look up at the speaker for ~3 s (a safe window to eat fast). A 💥 pencil-case crash makes the teacher turn quickly with only a short warning, but for a brief look.
9. Clear the desk before the bell to win. Stars: 1 for clearing, 2 for 20%+ of the time left, 3 for 40%+ left.

| Class | Snacks | Time | Turn every | Warning | Turn speed | Fake-out | New |
|---|---|---|---|---|---|---|---|
| 1 Math | 5 | 90s | 5–9s | 1.1s | 1.0s | 0% | Water sips |
| 2 Literature | 6 | 90s | 4.5–8s | 1.0s | 0.85s | 20% | Water sips |
| 3 English | 7 | 90s | 4–7.5s | 0.9s | 0.7s | 25% | Deskmate thief |
| 4 Physics | 8 | 85s | 3.5–7s | 0.8s | 0.55s | 30% | Surprise events |
| 5 History | 9 | 85s | 3–6s | 0.7s | 0.45s | 35% | Everything |

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
Edit `LEVELS` and `FOODS` at the top of the script in `index.html`: time, turn interval `turnEvery`, watch duration `watch`, warning length `warn`, turn speed `turnTime`, fake-out chance `fake`, water-sip chance `drink`, thief chance `thief`, event chance `events`, the snack list `items`, and sequence lengths.
