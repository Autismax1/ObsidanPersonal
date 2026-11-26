---
tags:
  - brotato/shop
---
# Weapon Rolls

[[Brotato]] › [[Shop Item Rolls]] › Weapon Rolls

> [!summary] At a glance
> - **Weapon slots:** exactly `2` in waves 1–2 (no `35%` roll), `1` guaranteed in waves 3–5, then `35%` per slot. A "minimum weapons in shop" effect raises the guarantee.
> - **Same weapon you own:** `23%` (+7% early, +2% per different weapon), then same class, else only new weapons.

^glance

## How many weapons
- Waves 1–2: weapon slots fill until the shop holds `max(2, minimum weapons in shop effect)` weapons, every other slot is an item.
- Locked weapons count toward the wave 1–2 guarantee.
- No weapons if your slots are full or an effect removes weapons from the shop.

## Which weapon
Each weapon slot makes one roll and lands in one of three bands:

| Band | Chance | Offers |
|---|---|---|
| Same weapon | 23% + early bonus + 2% per different weapon you own (max 6) | only weapons you already own |
| Same class | up to 35% + early bonus + 1% per different weapon, minus the same-weapon share | new weapons that share a class with yours |
| Anything else | the rest | only weapons you don't own |

- **Early bonus** shrinks by a fifth each wave and is gone from wave 6. At wave 1 it adds +20% to the same-class threshold.
- The public wiki still lists older values (20% same weapon, 15% same class, smaller early bonus). These numbers are from the current game code.
- Example, wave 1 with one weapon: 32% same weapon, 24% new weapon of the same class, 44% anything new.
- A fists build sees a lot of unarmed weapons early.

## Weapon tier limits
- Rarity rolls like items ([[Rarity Odds]]), clamped by min/max weapon tier effects.
- Some effects remove melee, ranged, duplicate or structure weapons.

## Cursed and meca weapons
- [[Curse#Curse chance]]
- [[Meca#Meca weapons in the shop]]
