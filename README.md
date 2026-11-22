# Operasi Bayang — Stealth Game

[![make.fun · best-stealth-game-20261121-1759](https://make.fun/badge/best-stealth-game-20261121-1759.svg)](https://make.fun/bounty/best-stealth-game-20261121-1759?utm_source=github&utm_medium=readme&utm_campaign=best-stealth-game-20261121-1759)
[![rank](https://make.fun/badge/best-stealth-game-20261121-1759/sakasaki919-cmd/best-stealth-game-20261121-2/rank.svg)](https://make.fun/bounty/best-stealth-game-20261121-1759/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=best-stealth-game-20261121-1759)
[![reward](https://make.fun/badge/best-stealth-game-20261121-1759/sakasaki919-cmd/best-stealth-game-20261121-2/reward.svg)](https://make.fun/bounty/best-stealth-game-20261121-1759?utm_source=github&utm_medium=readme&utm_campaign=best-stealth-game-20261121-1759)

Entry for the [make.fun](https://make.fun) bounty [best-stealth-game-20261121-1759](https://make.fun/bounty/best-stealth-game-20261121-1759) — "Make the best stealth game".

A top-down stealth game that plays offline in a desktop browser. Sneak through three guarded buildings, steal the loot, and reach the exit unseen.

## How to play

- **Move:** WASD or arrow keys. **Restart level:** R.
- **Guards** patrol fixed routes with vision cones. If a guard sees you, the detection meter fills and the guard gives chase; break line of sight or hide in bushes and shadows to lose them.
- **Objective:** collect all loot in the level, then reach the EXIT. Getting caught costs a life — you have three.
- **Levels:** 1. Gudang Senja, 2. Arsip Tengah Malam, 3. Bilik Brankas — more guards and faster patrols as you go.
- **HUD:** detection meter, lives, score, and level. Title, game-over, and victory screens included; sound effects are synthesized with WebAudio, no audio files.

## Run it

Open `game/index.html` directly in desktop Chrome — no build step, no dependencies, no network requests at all. A static server works too:

```sh
node serve.ts        # → http://localhost:8080
```

## Files

- `game/` — the playable game (HTML5 canvas, plain JavaScript, all files local)
- `screenshots/` — real renders of the game (title, gameplay, victory)
- `main.ts` — builds the submission dossier (`MAKEFUN_OUTPUT_DIR=out node main.ts`)
- `vendor/makefun-game.ts` — dossier helper from the competition kit, unchanged
