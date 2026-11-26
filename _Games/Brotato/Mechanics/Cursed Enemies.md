---
tags:
  - brotato/mechanic
  - brotato/enemy
  - brotato/dlc/abyssal-terrors
---
# Cursed Enemies

[[Brotato]] › [[Curse]] › Cursed Enemies · other variants: [[Evolved Enemies]]

> [!summary] At a glance
> - Chance per spawn: `50%·(1 − 1/(1 + curse/50))`. Bosses, elites and loot aliens never.
> - Stats: **+150% HP** (+2% per team curse), **+25% damage**, **+15% speed**, +33% materials.

^glance

## Chance per spawn
- Per player, averaged. Increased in endless.
- About 8% at 10 curse, 25% at 50, 33% at 100, never above 50%.
- Elites count as bosses in the code.

## Stats
| | Cursed |
|---|---|
| HP | **+150%** + 2% per point of **total team curse** (counted to 300, so max +750%) |
| Damage | +25% flat |
| Speed | +15% flat |
| Materials | +33% |

The script's defaults are higher (+200% / +50% / +75%), but the game's scene file overrides them with the values above.

- Items with "gold on cursed kill" or "bonus damage against cursed enemies" trigger here.
- In endless, curse also adds to the normal endless scaling of all enemies.
