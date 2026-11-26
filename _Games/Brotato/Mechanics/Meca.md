---
tags:
  - brotato/mechanic
  - brotato/dlc/primal-dread
---
# Meca

[[Brotato]] › [[Evolution]] › Meca · flowchart: [[Evolution Flow.canvas|Evolution Flow]]

> [!summary] At a glance
> - Mechanize a weapon for `meca rank + 1` (rank starts at 0) [[Evolution Drops#Meca parts|meca parts]]. Pick **1 of 2 stats** from two different groups.
> - Each rank adds meca power: `+3%` damage and stat scaling per power (1, 3, 6, 10…).
> - Same 4 stat groups for every weapon. Build damage always offers **your highest** damage stat.

^glance

The picked stat bonuses count toward your stats while you hold the weapon.

## One mechanize
1. **Pay** 1, then 2, then 3… parts. Any weapon that isn't cursed or mutant.
2. **Roll** from 2 **different** [[#The four stat groups|groups]]. The same stat again stacks.
3. **Meca power** + cost.
4. **First time only:** +1 evolution, weapon becomes meca.

## Meca power
Recalculated from the original weapon, not stacked:
- crit damage: **+2% per power**
- lifesteal: **+3% per power** (weapons that have some)
- structure weapons: damage and spawn rate

## The four stat groups
| Group | Stats | How the stat is picked |
|---|---|---|
| Defense | Max HP, Armor, Dodge, HP regen, Lifesteal | random |
| Support | Speed, Range, Luck, Harvesting | random |
| Damage | % Damage, Attack speed, Crit chance | random |
| Build damage | Melee, Ranged, Engineering, Elemental | **your highest**; ties go to what the weapon scales with |

- 2 of the 4 groups are drawn at random, so each group shows up about half the time.
- Skipped: dodge at the dodge cap, crit at the crit cap, and stats your character bans. Check your character in [[Characters]].

## Stat value by rank
Here Rn is the n-th mechanize of the weapon: it costs n parts and takes meca rank from n−1 to n.

| Stat | R1 | R2 | R3 | R4 | R5 | R6 | R7 | R8+ |
|---|---|---|---|---|---|---|---|---|
| Max HP · Dodge · Speed | 3 | 4 | 6 | 7 | 8 | 9 | 11 | 12 |
| Armor · Lifesteal · Ranged · Elemental | 1 | 1 | 2 | 2 | 3 | 3 | 4 | 4 |
| HP regen · Engineering | 2 | 2 | 3 | 3 | 4 | 4 | 5 | 5 |
| Range | 15 | 21 | 28 | 34 | 41 | 47 | 54 | 60 |
| Luck · Attack speed | 5 | 7 | 9 | 11 | 14 | 16 | 18 | 20 |
| Harvesting | 5 | 6 | 8 | 9 | 9 | 10 | 11 | 12 |
| % Damage | 5 | 6 | 8 | 9 | 11 | 13 | 14 | 16 |
| Crit chance | 3 | 4 | 5 | 6 | 6 | 7 | 8 | 9 |
| Melee | 2 | 3 | 4 | 5 | 5 | 6 | 7 | 8 |

R1 matches a common level-up, R8 a legendary one. Could be off by 1 where rounding lands on exactly .5.

## Combining and selling
- **Combining** two meca weapons adds their power and parts, keeps the higher rank and merges stat bonuses. No new choice.
- **Selling or recycling** refunds every part spent. See [[Prices and Rerolls#Recycling]].

## Meca weapons in the shop
```
chance = 81% × (1 − 1/(1 + evolution/70))     (evolution > 0)
```
- About 10% at +10, 24% at +30, 40% at +70.
- Arrives at rank 1. You pick its stat before buying.
- With both DLCs, the higher of evolution and curse rolls first. An item can't be both. See [[Curse#Curse chance]].
