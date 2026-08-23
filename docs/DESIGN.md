# Cascade design

Implement against this file, not folklore.

## Identity

- Product: **Cascade**
- Repo: `computerpets-cascade`
- Idea: Pet Puzzle Quest
- Genre: Match-3 RPG
- Engine: Phaser.js
- Surface: `8080`

## Loop

Matches are not just score. Red cluster = Rui swipe. Blue = Reed hop. The pet on the side of the board is yours, vitals-aware.

## Play beats

- Pick pet. Board colors map to its kit.
- Match to fill bars, tap to fire.
- Enemy is a training dummy or weekly boss.
- Win = treat + XP into Dojo, not a new mint.

## Neighbors

- computerpets (active pet)
- computerpets-quests
- computerpets-gambit (ability names)
- computerpets-telemetry

## Failure doctrine

Mis-tap spam → input debounce. Tab-out pauses vs dummy, disconnect vs boss. Colorblind palettes required.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
