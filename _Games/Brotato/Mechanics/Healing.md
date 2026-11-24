---
tags:
  - brotato/mechanic
---
# Healing

[[Brotato]] › Healing · tips: [[Lifesteal vs HP Regen]]

## Lifesteal
- **Every hit** rolls your lifesteal % as a chance to heal **1 HP**.
- Damage doesn't matter: a 5-damage hit and a 500-damage hit heal the same.
- **Cooldown 0.1 s**, so lifesteal heals at most **10 HP per second**.
- Expected healing: `hits per second × lifesteal %`, capped at 10 HP/s.
- Counts every weapon hit, so fast weapons, multiple projectiles, bounces and piercing all add rolls.

| Hits per second | 10% lifesteal | 20% lifesteal | 40% lifesteal |
|---|---|---|---|
| 2 | 0.2 HP/s | 0.4 HP/s | 0.8 HP/s |
| 10 | 1 HP/s | 2 HP/s | 4 HP/s |
| 30 | 3 HP/s | 6 HP/s | 10 HP/s (cap) |

## HP regeneration
- Heals **1 HP** every time a timer runs out, whether you hit anything or not.
```
timer = 5 s / (1 + (regen − 1) / 2.25)
```

| HP regen | 1 | 5 | 10 | 15 | 20 | 30 | 50 |
|---|---|---|---|---|---|---|---|
| Seconds per HP | 5.0 | 1.8 | 1.0 | 0.69 | 0.53 | 0.36 | 0.22 |
| HP per second | 0.2 | 0.56 | 1.0 | 1.44 | 1.89 | 2.78 | 4.56 |

- Grows in a straight line: every +2.25 regen adds 0.2 HP/s.
- 0 or negative regen: no regeneration at all.
- "Bonus HP regen below X% health" effects multiply the amount per tick.

## Characters that can't use one of them
See the table in [[Characters]] (banned item groups and banned meca stats). For example [[Golem]], [[Druid]] and [[Veteran]] lose lifesteal and regen items, and [[Vampire]] loses regen.
