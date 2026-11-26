---
tags:
  - brotato/drops
  - brotato/dlc/primal-dread
---
# Evolution Drops

[[Brotato]] › Drops · [[Evolution]] · related: [[Materials and Crates]]

> [!summary] At a glance
> - Meca/mutant fruit: flat `2%` per normal kill (no pity, no luck), your side only past `±2`.
> - Mutation fruit: `4%` per [[Evolved Enemies|mutant]] kill. Meca parts (`+2`): `2.5%` per [[Evolved Enemies|meca]] kill. Both have pity.
> - Each extra drop in the same wave makes the next one rarer: `÷(1 + 0.5 × dropped)`.

^glance

Four Primal Dread consumables. All four rolls happen on every kill that can drop consumables.

## Meca and mutant fruit
- **Effect:** meca fruit +1 evolution, mutant fruit −1 evolution.
- **Which one** (for the player who got the kill), first match wins:
  1. One type banned → the other.
  2. Meca only → meca. Mutant only → mutant.
  3. Dual evolution ([[Mad Scientist]]) → 50/50.
  4. Evolution **> +2** → meca. **< −2** → mutant.
  5. Otherwise → 50/50.

## Mutation fruit
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
- **Chance:** same formula as mutation fruit. No item requirement, no stat bonus.
- **Effect:** the parts are spent in the shop. See [[Meca]].
- **Other sources:**
  - Dismantling a shop weapon gives 1. See [[Prices and Rerolls#Dismantle (Primal Dread)]].
  - [[Droid]] gets 1 per level.
