# 🐾 Paws of Fury

A Mortal-Kombat-style **dog brawler** that runs entirely in the browser — one
self-contained `index.html`, HTML5 canvas + vanilla JS, no build step.

**▶ Play:** https://ross-code.github.io/paws-of-fury/

Pick your pup, fight best-of-three rounds, fill the special meter, and land a
comedic **FUR-TALITY** finisher when "FINISH THEM!" flashes.

## Roster

Each fighter has five stats — **strength, speed, agility, cleverness,
aggressiveness** — that drive real gameplay (damage, walk/dash speed, jump,
tankiness, CPU brain, and special-meter gain).

| Fighter | Breed | Identity | Special |
|---|---|---|---|
| **Elvis** | Siberian Husky (white) | All-round athlete | Sled Rush (dashing tackle) |
| **Dixie** | Blue Heeler | Clever, agile cattle-dog | Heel Nip (multi-hit dash bite) |
| **Lucy** | Doxie × Chihuahua | Tiny, long, **MAX aggression** + berserk rage | Rage Spin (spinning flurry) |
| **Houston** | Black German Shepherd | Heavy hitter / tank | Guard Slam (lunging body slam) |
| **Teenie** | Golden Doodle | Fluffy genius, zoner | Fur Puff (ranged projectile) |

Lucy's aggression is off-the-charts — her rage meter builds as she lands hits.

## Controls

| | Player 1 | Player 2 |
|---|---|---|
| Move | `A` / `D` | `◀` / `▶` |
| Jump | `W` | `▲` |
| Crouch | `S` | `▼` |
| Light attack | `F` | `,` |
| Heavy attack | `G` | `.` |
| Special (needs 50% meter) | `H` | `/` |
| Block | hold *away* from opponent | hold *away* from opponent |

Crouch + heavy = low sweep. Block lows by crouch-blocking. `M` mutes, `Esc`
returns to the menu.

- **1** — 1 Player vs CPU
- **2** — 2 Player local versus

## Run locally

It's a static file — open `index.html`, or:

```bash
npx serve -l 4312 .
# then visit http://localhost:4312
```

## Tech

No frameworks, no dependencies. Procedural dog art, WebAudio SFX + music,
fixed-timestep game loop, per-fighter AI tuned by the stat block.

Sibling project to [`elvis-escape`](https://github.com/ross-code/elvis-escape).
