---
tags:
  - brotato
  - brotato/index
---
# Run Cheat Sheet

[[Brotato]] › Run Cheat Sheet · your character: [[Characters]]

## Shop
| What | Value | More |
|---|---|---|
| Wanted tag roll | 5% of item rolls (10% boosted) | [[Shop Item Rolls#Wanted tags]] |
| Weapon slots | 2 guaranteed waves 1–2, 1 in waves 3–5, then 35% per slot | [[Weapon Rolls]] |
| Same weapon you own | 23% (+7% early, +2% per different weapon) | [[Weapon Rolls#Which weapon]] |
| Common floor | never below 40% | [[Rarity Odds]] |
| Legendary cap | 8% max | [[Rarity Odds]] |
| Legendary at wave 20 | 3% (6% at 100 luck) | [[Rarity Odds#Shop odds]] |
| Reroll | `int(0.75·wave) + d·(rerolls+1)`, `d = max(1, 0.4·wave)` | [[Prices and Rerolls]] |
| Recycling | 25% of price + recycling gains | [[Prices and Rerolls#Recycling]] |

## Drops
| What | Value | More |
|---|---|---|
| Materials | 100% until wave 4, then `1 − 1.5%·wave`, floor 50%; ×0.65 horde | [[Materials and Crates#Materials]] |
| Crate | falls off by `1/(1 + crates this wave)` | [[Materials and Crates#Crates]] |
| Meca / mutant fruit | 2% per normal kill | [[Evolution Drops#Meca and mutant fruit]] |
| Mutation fruit | 4% per mutant kill + pity | [[Evolution Drops#Mutation fruit]] |
| Meca parts | 2.5% per meca kill + pity | [[Evolution Drops#Meca parts]] |

## Healing
| What | Value | More |
|---|---|---|
| Lifesteal | lifesteal % chance per hit to heal 1 HP, max 10 HP/s | [[Healing#Lifesteal]] |
| HP regen | 1 HP every `5 s / (1 + (regen − 1)/2.25)`; 10 regen = 1 HP/s | [[Healing#HP regeneration]] |
| Which one | lifesteal for many hits, regen for few big hits | [[Lifesteal vs HP Regen]] |

## Structures and pets
| What | Value | More |
|---|---|---|
| Pet attack speed | never changes (your attack speed doesn't apply) | [[Structures and Pets]] |
| Turret attack speed | structure attack speed; [[Improved Tools]] adds 50% of your attack speed | [[Structures and Pets#Structure attack speed]] |

## Evolution
| What | Value | More |
|---|---|---|
| Side lock | past ±2 evolution: only your side's fruit and items | [[Evolution#The ±2 threshold]] |
| Mutation copy scale | `0.1 + 0.9·√(\|evo\|/130)` | [[Mutation#Copy strength]] |
| Pets copyable from | about −63 evolution | [[Mutation#Copy strength]] |
| Mechanize cost | rank + 1 parts | [[Meca]] |
| Meca damage | +3% per meca power | [[Meca#Meca power]] |
| Evolved enemy chance | `50%·(1 − 1/(1 + \|evo\|/50))` | [[Evolved Enemies]] |
| Evolved boss | always past ±30 team evolution | [[Evolved Enemies#Bosses and elites]] |

## Curse
| What | Value | More |
|---|---|---|
| Item cursed | `15%·(1 − 1/(1 + curse/50))` | [[Curse#Curse chance]] |
| Curse strength | `40% + 2%·min(20, wave−1) ± 30%`, so 10–70% at wave 1, 50–110% from wave 21 | [[Curse#Curse strength]] |
| Cursed values of one item | open it in [[Items]] / [[Weapons]] | |
| Enemy cursed | `50%·(1 − 1/(1 + curse/50))` | [[Cursed Enemies]] |
