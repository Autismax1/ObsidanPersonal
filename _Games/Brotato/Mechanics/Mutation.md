---
tags:
  - brotato/mechanic
  - brotato/dlc/primal-dread
---
# Mutation

[[Brotato]] › [[Evolution]] › Mutation · flowchart: [[Evolution Flow.canvas|Evolution Flow]]

> [!summary] At a glance
> - Needs **evolution < 0**. One mutation per mutation fruit, at **wave end**.
> - Picks a **random item** (your character counts, weapons never).
> - Coin flip: **delete a downside** of that item, or **copy a good effect** into the Tumor.
> - Copies scale with evolution: `0.1 + 0.9·√(|evo|/130)`. The Tumor always gets `−1` evolution.

A mutation picks one of your items and either **deletes one of its downsides** or **copies a good effect from your build into the Tumor**. The Tumor grows every time.

## When it happens
- Picking up a [[Evolution Drops#Mutation fruit|mutation fruit]] adds one pending mutation (not for meca-only characters).
- Pending mutations resolve at **wave end**.
- [[Variant]] also mutates at wave end automatically, and can mutate items as you buy them.
- **Needs evolution < 0** (dual evolution: anything but 0). Otherwise the fruit does nothing.

## Step 1: pick the item
- **Uniformly random** among your items.
- **Your character counts as an item.**
- Never picked: cursed or meca items, the Tumor, Axolotl, Builder turrets, Evolved Leap.
- **Weapons are never picked.**

## Step 2: better-tier roll (optional)
- Only with **Wildfire Mutation** (25%, legendary, max 1) or **Chimera Cells**.
- The item is replaced by a random item **one tier higher**, preferring one that shares a tag.
- The new item then goes through step 3.
- Never for characters, mutant items or legendaries.

## Step 3: remove or copy
The game builds two lists:
- **Removable:** negative effects on the picked item. Characters have none.
- **Copyable:** positive effects on **all** your items, including your character, but not the Tumor.

If both lists have entries, it flips a **coin**:
- **Remove:** one random downside is deleted and the item becomes mutant.
- **Copy:** one random good effect is copied, scaled down, and **added to the Tumor**. The picked item stays as it was.

### What counts as copyable
Not only plain stats. Any **positive** effect with a stat behind it qualifies, for example:
- weapon class bonuses ([[Brawler]]: unarmed +50% attack speed)
- "+X% gains of a stat"
- "+X stat for every Y", stat per wave or per level
- explosion and burn effects

Each character note lists exactly which of its effects can be copied.

### Never copyable
- **negative** effects, and effects the tooltip hides ([[Hidden Effects]])
- effects without a stat behind them (e.g. [[Romantic]]'s "melee weapons +50 range")
- price, reroll and shop effects (e.g. Coupon), starting items and weapons, mutation fruit chance
- on/off effects (e.g. dual evolution, meca only), multiply or convert effects, Builder effects
- stats already at their cap, chances already at 100%
- pets and structures below scale 0.7 (about −63 evolution)
- some strong effects also need scale 0.7: HP regen bonus, mutate-on-equip, better-tier mutation, projectiles on death, dig sites and a few others

## Copy strength
```
scale = 0.1 + 0.9 × √( min(|evolution|, 130) / 130 )
copied = ceil(source value × scale)
```
| \|evolution\| | 5 | 10 | 15 | 30 | 63 | 130+ |
|---|---|---|---|---|---|---|
| scale | 0.28 | 0.35 | 0.41 | 0.53 | 0.73 | 1.0 |
| +15 dodge copies as | +5 | +6 | +7 | +8 | +11 | +15 |

- Pets and structures need scale ≥ 0.7 (about −63 evolution).
- Example: [[Brawler]]'s +15 dodge at −12 evolution gives the Tumor +6 dodge.

## Step 4: the Tumor grows
- Mutation counter +1.
- **−1 evolution.**
- The copied effect, if any. Same-type effects merge into one line.
