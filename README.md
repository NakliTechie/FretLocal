# FretLocal

**Guitar fretboard note trainer.** Pick strings, pick a riff — it quizzes you on where each note lives. Single HTML file. No server, no account, no data leaving your device.

**[naklitechie.github.io/FretLocal](https://naklitechie.github.io/FretLocal)**

---

## What it does

- **Preset riffs** — load a famous riff (Smoke on the Water, Seven Nation Army, Come As You Are, Blackbird, Am Pentatonic) and drill those exact notes in order
- **Custom drill** — pick any 1–6 strings and set how many random reps
- **Find the note** — a note name appears; click the correct fret on each selected string, then hit Submit
- **Instant review** — frets light up: 🟢 correct hit · 🔴 wrong click · 🟠 missed the right fret
- **Score + breakdown** — per-rep table showing each string's result and time taken

## Sound

Karplus-Strong plucked string synthesis via the Web Audio API. Click a fret → hear the actual pitch of that string at that position. After each submission, the correct notes play so you hear what you were aiming for. No samples downloaded, no CDN — synthesised in ~30 lines of JS. Mutable via the 🔊 button.

## Fretboard

Frets 1–12 shown in standard tuning (E₂ · A₂ · D₃ · G₃ · B₃ · E₄). Each of the 12 chromatic notes appears exactly once per string in this range — no ambiguity, no open strings to trip over.

## Presets

| Preset | Artist | Strings | Notes |
|---|---|---|---|
| Smoke on the Water | Deep Purple | Low E | 12 |
| Seven Nation Army | The White Stripes | Low E | 7 |
| Come As You Are | Nirvana | D string | 10 |
| Blackbird (ascending run) | The Beatles | G + B | 9 |
| Am Pentatonic box 1 | — | Low E | 9 |

## Built with

| Layer | Tech |
|---|---|
| Sound synthesis | Web Audio API — Karplus-Strong |
| Rendering | Vanilla JS, CSS Grid |
| Storage | None |
| Hosting | GitHub Pages |

Zero dependencies. Zero build step. Open the file, it works.

---

Part of the **[NakliTechie](https://naklitechie.github.io)** series — browser-native tools that run entirely on your device.
