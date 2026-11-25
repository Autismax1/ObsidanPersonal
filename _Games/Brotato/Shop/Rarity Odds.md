---
tags:
  - brotato/shop
---
# Rarity Odds

[[Brotato]] › [[Shop Item Rolls]] › Rarity Odds

> [!summary] At a glance
> - Common never below `40%`, legendary never above `8%`.
> - Luck only multiplies the per-wave part. Late in a run it turns rares into legendaries.
> - Level-ups use your **level** instead of the wave. Levels 5/10/15/20 have fixed tiers.

## Formula
One random number per slot, checked from Legendary down:

```
chance(tier) = min(base + max(0, (wave − 1 − min_wave) × per_wave) × (1 + luck/100), max)
```

| Tier | Starts after wave | Per wave | Max |
|---|---|---|---|
| Tier 2 (uncommon) | 1 | +6% | 60% |
| Tier 3 (rare) | 3 | +2% | 25% |
| Tier 4 (legendary) | 7 | +0.23% | 8% |

- Luck only multiplies the per-wave part. Negative luck divides it.
- **Common never drops below 40%**, because the uncommon cap is 60%.
- **Legendary can never pass 8%** in the shop.

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

Late in a run, luck mostly turns rares into legendaries.

## Level-ups
- Level-ups use the same formula with your **level** in place of the wave.
- Fixed tiers: level 5 = uncommon, levels 10/15/20 = rare, every 5th level after 20 = legendary.
- Characters can ban level-ups. See your character note or [[Characters]].

## Crates
- Normal crates roll like a shop slot. Legendary crates are always tier 4.
- See [[Materials and Crates#Crates]].
