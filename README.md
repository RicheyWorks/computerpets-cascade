# Cascade

**Pet Puzzle Quest** — Match-3 battler that charges overlay pet abilities in real time.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

Matches are not just score. Red cluster = Rui swipe. Blue = Reed hop. The pet on the side of the board is yours, vitals-aware.

## Genre & engine

- Genre: **Match-3 RPG**
- Engine: **Phaser.js**
- Stack: TypeScript · Phaser 3 · match-3 board · real-time ability charge into a pet duel
- Default surface: `8080`

## How you play

1. Pick pet. Board colors map to its kit.
2. Match to fill bars, tap to fire.
3. Enemy is a training dummy or weekly boss.
4. Win = treat + XP into Dojo, not a new mint.

## Talks to

- computerpets (active pet)
- computerpets-quests
- computerpets-gambit (ability names)
- computerpets-telemetry

## Failure doctrine

Mis-tap spam → input debounce. Tab-out pauses vs dummy, disconnect vs boss. Colorblind palettes required.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Cascade must leave Rui walking.

## Layout

```
computerpets-cascade/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
cd app; npm install; npm run dev
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
