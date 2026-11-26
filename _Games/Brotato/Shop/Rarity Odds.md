---
tags:
  - brotato/shop
---
# Rarity Odds

[[Brotato]] › [[Shop Item Rolls]] › Rarity Odds

> [!summary] At a glance
> - **Common floor:** never below `40%` (because the uncommon cap is `60%`).
> - **Legendary cap:** `8%` max in the shop.
> - **Legendary at wave 20:** `3%` (`6%` at 100 luck).
> - Luck only multiplies the per-wave part (negative luck divides it). Late in a run it mostly turns rares into legendaries.
> - Level-ups use your **level** instead of the wave. Levels 5/10/15/20 have fixed tiers.

^glance

## Formula
One random number per slot, checked from Legendary down:

```
chance(tier) = min(base + max(0, (wave − 1 − min_wave) × per_wave) × (1 + luck/100), max)
```

| Tier | min_wave (first wave with a chance) | Per wave | Max |
|---|---|---|---|
| Tier 2 (uncommon) | 0 (wave 2) | +6% | 60% |
| Tier 3 (rare) | 2 (wave 4) | +2% | 25% |
| Tier 4 (legendary) | 6 (wave 8) | +0.23% | 8% |

## Shop odds
| | Common | Uncommon | Rare | Legendary |
|---|---|---|---|---|
| Wave 5, luck 0 | 76% | 20% | 4% | 0% |
| Wave 5, luck 100 | 52% | 40% | 8% | 0% |
| Wave 10, luck 0 | 46% | 40% | 13% | 0.7% |
| Wave 10, luck 100 | 40% | 35% | 24% | 1.4% |
| Wave 15, luck 0 | 40% | 36% | 22% | 1.8% |
| Wave 20, luck 0 | 40% | 35% | 22% | 3% |
| Wave 20, luck 100 | 40% | 35% | 19% | 6% |

## Level-ups
- Fixed tiers: level 5 = uncommon, levels 10/15/20 = rare, every 5th level after 20 = legendary.
- Characters can ban level-ups. See your character note or [[Characters]].

## Crates
- Normal crates roll like a shop slot. Legendary crates are always tier 4.
- See [[Materials and Crates#Crates]].
