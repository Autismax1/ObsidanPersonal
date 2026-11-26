---
tags:
  - brotato/mechanic
  - brotato/enemy
  - brotato/dlc/primal-dread
---
# Evolved Enemies

[[Brotato]] › [[Evolution]] › Evolved Enemies · other variant: [[Cursed Enemies]]

> [!summary] At a glance
> - Chance per normal enemy: `50%·(1 − 1/(1 + |evo|/50))`. About `8%` at ±10, `17%` at ±25, `25%` at ±50, never above `50%`.
> - Bosses are always evolved past `±30` team evolution, otherwise the normal chance. Elites get `4×` the chance (max 100%) to be swapped for a meca or mutant elite.
> - Meca enemies drop **meca parts** (`2.5%`), mutant enemies drop **mutation fruit** (`4%`).

^glance

Meca and mutant enemies both come from one shared roll.

## Chance per normal enemy
```
w      = |evolution| × (1 + enemy evolution chance %)
chance = 50% × (1 − 1/(1 + w/50))
```
- Averaged over players. Increased in endless.

## Which side
- Weighted by evolution: meca players' evolution against mutant players' |evolution|.
- Dual evolution counts toward both.
- Solo, you only get your own side.

## Bosses and elites
- Enemies spawned by an evolved enemy share its side. Loot aliens never evolve.

## Stats
Strength = the average |evolution| of that side's players.

| | Meca | Mutant |
|---|---|---|
| HP | +50% + 2% per evolution (counted to 300) | +25% + 2.4% per evolution (counted to 300) |
| Damage | +25% → +50% (square-root curve, 1–100 evo) | +15% → +80% (linear, 1–150 evo) |
| Speed | +5% → +25% (square-root curve, 1–100 evo) | +5% → +25% (square-root curve, 1–100 evo) |
| Materials | +33% | +33% |
| Special drop | [[Evolution Drops#Meca parts\|meca parts]] 2.5% | [[Evolution Drops#Mutation fruit\|mutation fruit]] 4% |

- Evolved enemies never drop [[Evolution Drops#Meca and mutant fruit|meca or mutant fruit]].
- Items with "material on evolved kill" or "heal on mutant kill" trigger here.
