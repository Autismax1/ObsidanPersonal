---
tags:
  - brotato/weapon
  - brotato/weapon/ranged
  - brotato/dlc/primal-dread
type: Ranged
classes:
  - Precise
lowest_tier: 1
damage_lowest_tier: 10
cooldown_lowest_tier: 0.80
dlc: Primal Dread
---

# Carbon Bow

[[Brotato]] › [[Weapons]] · **Ranged** · Primal Dread

> [!info] Weapon
> **Classes** [[Weapon Classes#Precise|Precise]] · **Tiers** 1–4 · shop odds: [[Weapon Rolls]] · [[Meca|mechanizable]] unless cursed or mutant
> **Starting weapon choice for** [[Apprentice]], [[Archaeologist]], [[Baby]], [[Buccaneer]], [[Captain]], [[Chunky]], [[Curious]], [[Cyborg]], [[Diver]], [[Droid]], [[Engineer]], [[Entrepreneur]], [[Explorer]], [[Fisherman]], [[Gangster]], [[Generalist]], [[Glutton]], [[Hiker]], [[Hunter]], [[Jack]], [[King]] (tier 2), [[Lich]], [[Loud]], [[Lucky]], [[Mad Scientist]], [[Masochist]], [[Multitasker]], [[Mutant]], [[Old]], [[One Armed]], [[Poacher]], [[Ranger]], [[Renegade]], [[Romantic]], [[Saver]], [[Sick]], [[Soldier]], [[Streamer]], [[Survivor]], [[Technomage]], [[Time Shifter]], [[Vampire]], [[Variant]], [[Veteran]], [[Well Rounded]], [[Wounded]]

## Stats per tier
**All tiers** Range 350 · Knockback 0 · Accuracy 100%

| Tier | Price | Damage | Scaling | Cooldown (0 attack speed) | Crit |
|---|---|---|---|---|---|
| 1 | 18 | **10** | 70% Ranged damage | 0.80s | 30% ×1.5 |
| 2 | 37 | **12** | 85% Ranged damage | 0.77s | 35% ×1.5 |
| 3 | 68 | **15** | 100% Ranged damage | 0.73s | 40% ×1.75 |
| 4 | 145 | **18** | 110% Ranged damage | 0.70s | 45% ×1.75 |

## Effects per tier
Each shot randomly scales with one damage stat; what the shot does depends on that stat.

| Effect | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|---|---|---|---|---|
| **Random damage stat per shot** (`Carbon bow random scaling`) | ✓ | ✓ | ✓ | ✓ |
| **Melee shot: slows the enemy by 50%, wearing off over** (`Carbon bow melee, while it scales with Melee damage (+50)`) | 0.5s | 1s | 1.5s | 2s |
| **Ranged shot: extra piercing** (`Carbon bow ranged, while it scales with Ranged damage`) | +1 | +1 | +2 | +2 |
| **Elemental shot: Burning … (100% Elemental damage)** | 3×3 | 5×5 | 8×6 | 12×9 |
| **Engineering shot: chance on hit to drop a landmine** (`Carbon bow engineering, while it scales with Engineering`) | 2% | 3% | 4% | 5% |

Landmine, all tiers: structure: `10` damage (100% Engineering) · every `0.23s` · Explodes on hit (100% chance, explosion size 175%). Its data also has a "spawns every 12s" timer, which doesn't apply here: the bow drops mines on hit.

> [!note] Structures
> Its structures use structure % damage, structure range and **structure attack speed** (e.g. [[Improved Tools]]). See [[Structures and Pets]].

## Cursed
Worst → best roll, see [[Curse#Curse strength]]. Each effect rolls on its own.

| Tier | Damage | Scaling | Crit damage | Curse stat added |
|---|---|---|---|---|
| 1 | `11 → 21` | 77% → 147% Ranged damage | ×1.5 → ×1.8 | `+1 → 2` |
| 2 | `14 → 26` | 94% → 178% Ranged damage | ×1.5 → ×1.8 | `+2 → 3` |
| 3 | `17 → 32` | 110% → 210% Ranged damage | ×1.8 → ×2.1 | `+3 → 6` |
| 4 | `20 → 38` | 121% → 231% Ranged damage | ×1.8 → ×2.1 | `+6 → 12` |

**Effects when cursed** (value; every effect also gets burn and structure damage `×1.10 → ×2.10`)

| Effect | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|---|---|---|---|---|
| Carbon bow random scaling | `0` | `0` | `0` | `0` |
| Carbon bow melee (+50) | `56 → 105` | `56 → 105` | `56 → 105` | `56 → 105` |
| Carbon bow ranged | `2 → 3` | `2 → 3` | `3 → 5` | `3 → 5` |
| Burning | `0` | `0` | `0` | `0` |
| Carbon bow engineering | `3 → 5` | `4 → 7` | `5 → 9` | `6 → 11` |
