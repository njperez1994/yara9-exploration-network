# System Overview: Macana YARA-9 Exploration Network

## Vision

Macana Corp is building a gameplay-driven intelligence economy for EVE Frontier. The objective is to discover and operationalize YARA-9 intelligence by combining exploration, validation, and utility-focused rewards.

The system is designed to feel like a real corporate network: players generate strategic mineral data, Macana validates the data, and rewards are issued through an internal utility currency (MTC) that unlocks meaningful services.

## Problem

- Valuable exploration activity often feels disconnected from long-term progression.
- Rewards can become repetitive when they are not tied to infrastructure access or strategic utility.
- Rare-resource discovery loops are hard to balance without anti-abuse controls.

## Solution

Macana introduces a modular loop where exploration output becomes an economic input:

`Acquire Satellite -> Scan Target -> Retrieve Data Item -> Redeem at MCC -> Receive Standing and Rewards -> Progress`

This loop links player action to a controlled progression economy instead of isolated loot events.

## Core Components

### 1) Satellite and License Layer

- Tier 1 satellites are fabricated by Macana Corp with in-game resources.
- Tier 1 public access is capped per player per 24h based on standing.
- Tier 2 and Tier 3 require a consumable license item per satellite crafted.
- Licenses are crafted at MCC from base resources and can be traded.
- Better equipment improves probability and value, not guaranteed outcomes.

### 2) Scan and Data Layer

- Players scan rocky celestial bodies.
- Outputs are categorized as:
  - Common Mineral Data
  - Rare Mineral Data
  - YARA-9 Signature Fragments
- Result quality depends on tier, scan duration, and balancing parameters.

### 3) Macana Commerce Center

The Commerce Center acts as:

- distribution center (satellite access and licensing)
- exchange point (data redemption for MTC)
- industrial gateway (higher-tier progression)
- infrastructure access authority (stations, routes, restricted services)

Access model:

- neutral players can access MCC
- hostile players are denied
- higher standing improves pricing conditions and access tiers

### 4) Validation and Economy Layer

Before rewards are issued, submitted data is validated using eligibility rules:

- satellite tier and class
- target context
- data rarity category
- duplication checks
- reward policy state
- duplication window state

Validation outputs are represented as real data items (with source and timestamp metadata) that can be lost in transit if a carrier is destroyed.

MTC is distributed from a daily budget linked to Macana treasury performance in LUX, then allocated by weighted data value.

## Why This Matters

The design creates a closed utility loop where token value comes from in-system demand: access, upgrades, mobility, and corporate services, while emission remains budget-controlled.

This gives the project two strengths for long-term adoption:

1. Immediate gameplay readability.
2. A credible path to on-chain validation without changing core identity.

## Macana Lore Foundation

Macana Corp is positioned as an industrial intelligence operator, not only a resource trader. Its role is to coordinate exploration logistics, validate strategic data, and convert information into operational value.

This narrative frame supports the gameplay model: players are not only collecting minerals, they are contributing to a corporate intelligence network focused on YARA-9 discovery.

## Implementation Path

### Current Stage

- Concept and architecture defined.
- Visual direction and loop design prepared.
- Reward and validation logic scoped.

### Next Stage

- Web-based interactive prototype of the exploration loop.
- Simulated scan outcomes, failures, and redemption flow.
- Standing-based Tier 1 distribution limits and cooldowns.
- Dynamic reward simulation from weighted score and daily budget.

### Future Stage

- Smart contract implementation on Sui for validation and rewards.
- Rule enforcement for licensing and infrastructure permissions.
- Iterative balancing based on player testing data.

## Success Criteria (Prototype)

- A first-time user can complete a compressed demo scan-to-progress cycle in about 3 minutes.
- A full in-world cycle (acquire, travel, scan, return, redeem) has a realistic target window that includes travel and risk.
- Tier 1 anti-hoarding limits are visible and understandable.
- Reward value changes dynamically based on data quality and duplication.
- Understand the MVP loop and future scalability path in one walkthrough.
