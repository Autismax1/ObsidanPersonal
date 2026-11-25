---
tags:
  - brotato/shop
---
# Prices and Rerolls

[[Brotato]] › [[Shop Item Rolls]] › Prices and Rerolls

> [!summary] At a glance
> - Price: `(base + wave + base × wave × 0.1) × (1 + price%)`.
> - Reroll: `int(0.75·wave) + d·(rerolls + 1)`, with `d = max(1, int(0.4·wave))`.
> - Recycling gives `25%` of the price, plus recycling gains.

## Item price
```
price = (base + wave + base × wave × 0.1) × (1 + items price %)
```
- Weapons also apply weapons price %.
- [[Danger Levels#Danger 6 (Nightmare)|Nightmare]] raises the 0.1 to 0.11, a hidden effect. See [[Hidden Effects]].
- In endless, prices grow with the endless factor.

## Reroll price
```
d = max(1, int(0.4 × wave))
reroll = int(0.75 × wave) + d × (rerolls this shop + 1)
```
- Reroll price % reduces it, down to 10% at most.

## Recycling
- You get **25% of the item's current price**, plus recycling gains %.
- An item worth 1 always recycles for 1.
- Selling a meca weapon also refunds every meca part spent on it. See [[Meca]].

## Dismantle (Primal Dread)
- Pay gold (base 11, scales with wave) to turn a shop weapon into **1 meca part**. See [[Evolution Drops#Meca parts]].
