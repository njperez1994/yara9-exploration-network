# Architecture Overview

The **YARA-9 Exploration Network** is designed as a modular exploration, validation, and economic utility system built around Macana Corp’s search for YARA-9.

Its architecture is divided into four functional layers:

1. **Player Interaction Layer**
2. **Satellite Scan Logic Layer**
3. **Macana Commerce Center Layer**
4. **Economic and Validation Layer**

This structure allows the project to begin as a strong visual and systems prototype, while also defining a clean path toward future implementation on Sui.

---

## 1. Player Interaction Layer

This layer represents the player-facing experience inside the Macana Commerce Center and future connected interfaces.

### Main Player Actions

- Acquire a Tier 1 satellite from Macana public distribution (quota-based)
- Review advanced satellite tiers and licensing requirements
- Launch scans against rocky celestial bodies
- Receive mineral intelligence data
- Deliver recovered data to Macana Corp
- Exchange validated data for **Macana Trading Coin (MTC)**
- Spend MTC on services, access, upgrades, and infrastructure

### Design Goal

Keep the system readable and satisfying from the first interaction.

Core loop:

`Acquire → Scan → Retrieve Data → Redeem → Spend → Progress`

This is the layer most visible to the players, so it should feel immediate, understandable, and tied to a larger economic purpose.

---

## 2. Satellite Scan Logic Layer

This layer defines how scanning satellites behave and how mineral intelligence is generated.

Satellites are not treated as simple random loot devices. They are structured exploration tools with different performance profiles, progression paths, and strategic trade-offs.

### Satellite Classes

#### Tier 1 Satellite

- Fabricated by Macana Corp using in-game resources
- Publicly distributed under per-player daily quota rules
- Low scan precision
- Lower-value or broader scan output
- Beginner-friendly onboarding tool
- Designed to introduce players into the YARA-9 exploration loop

#### Advanced Tier Satellites

- Unlocked through licenses and industrial crafting
- Higher scan precision or specialization
- Better access to rare or strategic data outputs
- Balanced with trade-offs such as cost, build requirements, or longer scan cycles
- Tier 3 introduces persistent operation, fuel consumption, and heat/visibility risk

### Scan Output Categories

- **Common Mineral Data**
- **Rare Mineral Data**
- **YARA-9 Signature Fragments**

### Potential Scan Variables

The system can be balanced around variables such as:

- satellite tier
- target body type
- scan duration
- signal fidelity
- region modifiers
- cooldown state
- validation threshold

### Design Goal

The scan layer should create opportunity, not certainty.

Better equipment improves the quality and strategic value of outcomes, but does not guarantee premium results. This keeps progression meaningful while preserving room for balancing.

---

## 3. Macana Commerce Center Layer

The **Macana Commerce Center** is the operational center of the whole network.

It functions as:

- industrial hub
- exchange point
- distribution center
- service gateway
- narrative anchor for Macana Corp

### Core Functions

#### A. Satellite Distribution

- Provide quota-limited Tier 1 satellites fabricated by Macana
- Present advanced licensing paths
- Support progression into higher-tier exploration

Standing-based distribution profile example:

- low standing: up to 5 Tier 1 per 24h
- mid standing: up to 10 Tier 1 per 24h
- high standing: up to 15 Tier 1 per 24h

#### B. Data Redemption

- Receive scan data from players
- Classify and validate the submission
- Exchange accepted intelligence for MTC

#### C. Industrial Services

- Support higher-tier satellite production
- Provide licensing and construction pathways
- Create controlled progression into specialized equipment

#### D. Infrastructure Access

- Offer access to Macana-controlled stations
- Unlock gates, routes, or internal trade options
- Expand the practical value of MTC beyond a simple reward token

### Design Goal

The hub should feel like a real corporate ecosystem.

Players are not just cashing in a reward. They are participating in the infrastructure of a corporation that trades in mineral intelligence, industrial access, and strategic mobility.

---

## 4. Economic and Validation Layer

This layer governs trust, rewards, and long-term sustainability.

It is the most important layer for the future on-chain direction of the project.

### Validation Logic

Before scan data is exchanged for MTC, the system should validate:

- satellite tier used
- target context
- data category
- reward eligibility
- duplication rules
- strategic weight of the result

### Reward Logic

MTC rewards are based on:

- data rarity
- satellite capability
- scan quality
- strategic value
- current balancing rules
- daily mint budget policy linked to Macana LUX stock performance
- duplication penalty windows

### Token Utility

MTC gains value through internal usefulness, including:

- discounts on ships and minerals
- access to stations and gates
- industrial permissions
- satellite upgrades
- specialized Macana services

### Anti-Abuse Considerations

To prevent value collapse and repetitive farming, the full implementation should account for:

- duplicate scan suppression
- duplicate value decay in short windows
- diminishing returns
- low-value output throttling
- controlled reward curves
- premium access restrictions

### Design Goal

MTC is not intended to function as an empty speculative token.

Its value comes from access, infrastructure, service demand, and the controlled redemption of exploration intelligence.

---

## 5. Future On-Chain Implementation

The current architecture is intentionally designed so it can evolve into a Sui-based system without changing its core gameplay identity.

### Future Smart Contract Roles

- register satellite classes
- validate redemption events
- issue MTC rewards
- enforce licensing rules
- manage infrastructure access permissions
- support scalable corporate service systems

### Implementation Vision

In a future deployed version, scan-related actions would generate economically meaningful outcomes tied to Macana Corp’s infrastructure and internal currency model.

This creates a bridge between narrative design, gameplay systems, and on-chain validation.

---

## 6. High-Level System Flow

`Player acquires satellite`  
→ `Player scans rocky celestial body`  
→ `System produces mineral intelligence data item`  
→ `Player delivers data to Macana Commerce Center`  
→ `Validation layer checks reward eligibility`  
→ `Player receives MTC`  
→ `Player spends MTC on services, access, upgrades, or infrastructure`

---

## 7. Architecture Summary

The **YARA-9 Exploration Network** is built around three core pillars:

- **Exploration** through orbital satellites
- **Validation** through Macana corporate infrastructure
- **Utility** through MTC as a functional internal currency

We hope this architecture makes the project credible both as a hackathon prototype and as a future live economic system within EVE Frontier.
