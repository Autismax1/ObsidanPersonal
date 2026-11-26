---
tags:
  - brotato/mechanic
---
# Structures and Pets

[[Brotato]] › Structures and Pets · related: [[Items]], [[Weapons]]

> [!summary] At a glance
> - Pets are **not** structures. **Nothing** changes a pet's attack speed, not your attack speed and not [[Improved Tools]].
> - Structures use **structure attack speed**. [[Improved Tools]] adds `50%` of your attack speed to it.
> - Turrets shoot every `70–130%` of their cooldown (random).

^glance

The game builds pet stats differently from structure stats, and attack speed is where it matters most.

## Which stats they get
| | Structures (turrets, landmines, garden…) | Pets (Bonk Dog, Catling Gun, Mosquitor…) | Structure pet ([[Bot O Mine]]) |
|---|---|---|---|
| % Damage | no, only **structure % damage** | yes | yes, **plus** structure % damage |
| Crit chance | only with a "structures can crit" effect | yes | only with "structures can crit" |
| Range | structure range | your range (melee pets: half of it) | structure range |
| Your attack speed | no | **no** | **no** |
| Structure attack speed | **yes** | no | no (see below) |

## Structure attack speed
```
structure attack speed = structure attack speed stat + (share of your attack speed from effects)
cooldown = cooldown / (1 + structure attack speed)     if positive
cooldown = cooldown × (1 + |structure attack speed|)   if negative
```
- **[[Improved Tools]]** example: with 100 attack speed that's +50% for turrets.
- **Negative attack speed** with Improved Tools makes turrets **slower**.
- Applied to: turret attack cooldowns, and spawn timers of structures that spawn on a timer, like [[Landmines]] and [[Screwdriver]] mines.

## Pets and attack speed
- The game sets attack speed to 0 when it builds pet stats.
- Pets count their timers in ticks (60 per second), so the cooldowns on the pet notes are their real attack intervals.
- **[[Bot O Mine]]:** its tooltip applies structure attack speed to the landmine timer, but the pet itself uses the raw 5 s. With Improved Tools the tooltip shows a shorter time than you actually get.
