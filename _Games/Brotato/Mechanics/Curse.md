---
tags:
  - brotato/mechanic
  - brotato/dlc/abyssal-terrors
---
# Curse

[[Brotato]] › Abyssal Terrors · enemies: [[Cursed Enemies]]

> [!summary] At a glance
> - **Chance** an item is cursed: `15%·(1 − 1/(1 + curse/50))`. `0` curse = no cursed items.
> - **Strength**: `40% + 2%·min(20, wave − 1) ± 30%`, so `10–70%` at wave 1 and `50–110%` from wave 21.
> - Good values ×(1 + strength), bad values ÷(1 + strength). Each effect rolls separately.

A cursed item multiplies its good values and divides its bad values by the same random modifier. **Your curse stat only decides whether things get cursed.** Strength depends on the wave and the roll.

## Curse chance
Rolled once for every shop or crate item:
```
chance = 15% × (1 − 1/(1 + curse/50))
```
| Curse | 0 | 10 | 25 | 50 | 100 | 200 | ∞ |
|---|---|---|---|---|---|---|---|
| Item cursed | 0% | 2.5% | 5% | 7.5% | 10% | 12% | 15% |

- **0 curse means no cursed shop items.**
- Never cursed: items already cursed, meca or mutant.
- With both DLCs, the higher of curse and evolution rolls first. See [[Meca#Meca weapons in the shop]].

### Other ways to get curses
- Locked items with **Fish Hook** (own pity counter)
- Cursed starting items
- Dino eggs hatching
- **Ammosaurus**
- Combining a cursed weapon

## Curse strength
```
modifier = 40% + 2% × min(20, wave − 1) + random(−30 … +30)%
```
- **Weapons:** one roll for damage and scaling ×(1 + m), crit damage ×(1 + m/5), pierce and bounce +1 at most.
- **Every effect rolls on its own:** good values ×(1 + m) rounded up, bad values ÷(1 + m).
- The **shown curse level is the highest roll**, so items with many effects show higher curses.

| Wave | Lowest | Average | Highest |
|---|---|---|---|
| 1 | 10% | 40% | 70% |
| 5 | 18% | 48% | 78% |
| 10 | 28% | 58% | 88% |
| 15 | 38% | 68% | 98% |
| 20 | 48% | 78% | 108% |
| 21+ | 50% | 80% | 110% |

Exact cursed values per item and weapon: open the item in [[Items]] or the weapon in [[Weapons]].

The public wiki writes the wave part as `2% × min(wave, 20)`. The current game code uses `min(20, wave − 1)`, so the code's values are 2 points lower until wave 21.

## Why low curses show up late
- **±30 is wider than all the wave growth.** A late-game worst roll (50%) is no better than an average wave-5 roll (48%).
- **Single-effect items** get one roll and land low more often.
- **Fixed 38%:** starting items, dino eggs and Ammosaurus ignore wave and randomness.
- **Combining** re-rolls, but never below the higher of the two inputs.
- **Locked items** keep the roll from the shop they first appeared in.
