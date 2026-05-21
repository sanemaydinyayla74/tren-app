# Tren — Turkish, piece by piece

A small puzzle game that teaches Turkish word structure (suffixes, case endings, possessives) by building word "trains."

🚂 **Try it:** [URL coming after deploy]

## What it does

Turkish is an agglutinative language — words stack endings to add meaning:
- **ev** (house) → **evler** (houses) → **evlerim** (my houses) → **evlerimden** (from my houses)

Each ending follows a fixed order. This app turns that order into a train: locomotive (root) + wagons (endings).

Players see an English meaning ("from my houses"), choose the right wagons in order, and watch the Turkish word appear piece by piece. Soft consonant changes (p→b, k→ğ, t→d, ç→c) animate live.

## Current state

- ✅ 15 puzzles, graduated difficulty
- ✅ Soft consonant (yumuşama) animation system
- ✅ Hearts + streak + stars
- ✅ PWA: works offline, installable on home screen
- ⏳ Planned: 100+ puzzles, verb conjugation train, audio, daily challenge

## Tech

- Vanilla HTML/CSS/JS (no framework, no build step)
- PWA with manifest + service worker
- Web fonts: Fraunces + Nunito

## For testers

Honest feedback wanted on three questions:
1. Did you finish all 15 puzzles?
2. What clicked? What confused you?
3. Would you use this every day to learn Turkish?

## Local development

Just open `index.html` in a browser. No build, no install.

For PWA testing (service worker needs HTTPS), serve locally:
```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## License

All rights reserved (for now — open source TBD).
