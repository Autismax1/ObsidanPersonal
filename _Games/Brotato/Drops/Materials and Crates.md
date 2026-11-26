---
tags:
  - brotato/drops
---
# Materials and Crates

[[Brotato]] › Drops · related: [[Evolution Drops]]

> [!summary] At a glance
> - Materials: `100%` in waves `1–4`, then `1 − 1.5%·wave` from wave `5` (floor `50%`). Horde waves `×0.65`.
> - Crate chance is divided by `1 + crates already dropped this wave`.
> - Luck counts **added up across players** in co-op.

^glance

## Materials
- Wave 10: 85%. Wave 20: 70%.
- Elites and bosses always drop.
- Meca, mutant and cursed enemies give **+33% material value**. See [[Evolved Enemies]], [[Cursed Enemies]].

## Consumables
Every kill first rolls for a consumable:
```
consumable = enemy base chance × (1 + luck)
```
- Most enemies: 1%. Trees: 100%. Elites and bosses: always.
- In endless this is divided by `(1 + endless factor)`.
- If no consumable drops, fruit-drop effects (Fruit Basket etc.) get their own roll.

## Crates
If a consumable drops, it becomes a crate with:
```
crate = enemy crate chance × (1 + luck) × (1 + crate %) / (1 + crates dropped this wave)
```
- The second crate this wave is half as likely, the third a third.
- Trees: 20% crate before the falloff.
- Bosses drop a **legendary crate** (before endless).
- Dig sites can dig up crates, with their own falloff.

## Fruit
- Poisoned fruit effects can swap a normal fruit for poisoned fruit.
- Evolution consumables have their own rolls: [[Evolution Drops]].
