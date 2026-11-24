---
tags:
  - brotato/drops
  - brotato/dlc/primal-dread
---
# Evolution Drops

[[Brotato]] › Drops · [[Evolution]] · related: [[Materials and Crates]]

Four Primal Dread consumables. All four rolls happen on every kill that can drop consumables.

## Meca and mutant fruit
- **Who drops it:** normal enemies only. Meca and mutant enemies never drop it.
- **Chance:** flat **2%** per kill. No pity, no luck.
- **Effect:** meca fruit +1 evolution, mutant fruit −1 evolution.
- **Which one** (for the player who got the kill), first match wins:
  1. One type banned → the other.
  2. Meca only → meca. Mutant only → mutant.
  3. Dual evolution ([[Mad Scientist]]) → 50/50.
  4. Evolution **> +2** → meca. **< −2** → mutant.
  5. Otherwise → 50/50.

## Mutation fruit
- **Who drops it:** [[Evolved Enemies|mutant enemies]] only.
- **Needs:** one player with 3+ items that can mutate (not counting the character).
- **Chance:**
  ```
  chance = min(1, 4% × pity × (1 + bonus%)) / (1 + 0.5 × dropped this wave)
  pity   = 1 + misses / 20
  ```
- **Pity** is kept across waves and resets when a fruit drops.
- **Bonus** is the mutation fruit chance stat, e.g. [[Mad Scientist]]'s hidden +100%.
- **Endless:** the 4% base drops 1 point every 10 waves, to 1%.
- **Effect:** one mutation at wave end. See [[Mutation]].

## Meca parts
- **Who drops it:** [[Evolved Enemies|meca enemies]] only.
- **Chance:** same formula with a **2.5%** base. No item requirement, no stat bonus.
- **Effect:** meca parts to spend in the shop. See [[Meca]].
- **Other sources:**
  - Dismantling a shop weapon gives 1. See [[Prices and Rerolls#Dismantle (Primal Dread)]].
  - [[Droid]] gets 1 per level.
