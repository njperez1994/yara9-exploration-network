# Macana Corp: YARA-9 Exploration Network

Gameplay-driven exploration and intelligence economy for EVE Frontier.

*Hackathon Prototype – Active Development*

## Objective

Build a practical exploration loop where players generate scan data, redeem it through Macana infrastructure, and progress through utility systems instead of one-off loot outcomes.

## Lore Foundation

Macana Corp traces its origin to DrZeus, an industrial engineer linked to nickel and cobalt operations in Moa, where YARA-9 was first studied as a strategic material.

YARA-9 enabled breakthroughs in conductivity, fusion-adjacent processes, and gravitational stabilization for warp-scale systems, but prolonged exposure also altered human cognition and degraded biological limits.

After the convergence events represented in EVE Frontier, DrZeus and allied researchers from the YARA Team transitioned their consciousness into new operational bodies. In this universe, Macana Corp was founded to locate and control YARA-9, leverage its advantages as a faction, and pursue a long-term objective: determine whether a return path to their origin universe can eventually be engineered.

## Core Loop

`Acquire Satellite -> Scan Planet -> Retrieve Data Item -> Redeem at MCC -> Receive Standing and Rewards -> Progress`

## Key Design Decisions

- Tier 1 satellites are fabricated by Macana Corp using in-game resources (no spawning).
- Tier 1 public distribution is limited per player per 24h, based on standing.
- Tier 2/Tier 3 satellites require a consumable license item per unit crafted.
- Licenses are crafted in MCC from base resources and can be traded.
- Neutral players can access MCC; hostile players are denied.
- Higher standing unlocks better prices and selected subsidized goods.

## Satellite Tiers

- `Tier 1`: onboarding scan unit, low-value outputs, supports standing progression.
- `Tier 2`: higher-value data potential, stronger reward profile.
- `Tier 3`: persistent scanner with fuel cost and heat management, but detectable emissions increase PvP risk.

## Data and Rewards

- Scan outputs become real data items that can be lost if the carrier ship is destroyed.
- Reward value is dynamic, not fixed, and depends on rarity, quality, demand, freshness, and duplication penalty.
- MTC emission is budget-based and backed by Macana economic performance in LUX.

## Currency Model

- Hybrid economy: LUX (base market/crafting) + MTC (Macana utility and premium services).
- MTC can recirculate through corporate sinks, with optional burn mechanics for supply control.

## Current Focus

- Lock documentation for a coherent v1 ruleset.
- Build a simple interactive web prototype for scan mechanics and redemption.
- Validate two timing targets before deeper on-chain scope:
  - compressed demo loop: about 3 minutes
  - in-world operational loop: target range based on travel and risk

## Team

- Zeus1994 - System Design, Narrative, Economy Architecture

## Media and Community

- DrZeus story arc (Mambi Espacial): https://www.youtube.com/playlist?list=PLs9Qsj8c8_C3fav3oNHz7juBbBpw2-Cmq
- EVE Frontier | Mas que un juego: https://www.youtube.com/playlist?list=PLs9Qsj8c8_C2kLLuve01XkKXFzPH6HXv4
- EVE Frontier, Progresion en Espanol: https://www.youtube.com/playlist?list=PLs9Qsj8c8_C3MY7VaLkpEyIWAL4Iw22n5

## Design Philosophy

Macana Corp does not only sell resources.
Macana sells intelligence about where value exists.

Control the data...control the Frontier.

## Intellectual Property Notice

Macana Corp, YARA-9, the Exploration Network concept, and all associated systems, designs, and narrative elements are original creations by njperez1994.

All rights reserved.
