# Tokenomics: Macana Trading Coin (MTC)

## Token Role

MTC is a utility token inside the Macana exploration network. It is not designed as a speculative asset. Its value is created by practical demand in gameplay and infrastructure access.

Primary purpose:

- reward validated exploration intelligence
- unlock progression services
- gate premium access and operational privileges

## Utility Design

Players use MTC for:

- satellite upgrades and specialized scan modules
- licensing for advanced satellite tiers
- discounts on ships and minerals in Macana services
- access to stations, routes, and restricted corporate zones
- participation in high-value contracts and strategic missions

## Emission Budget (LUX-Backed)

MTC issuance is budget-governed, not infinite.

- Macana treasury tracks economic performance in LUX.
- A daily MTC emission cap is set from treasury policy.
- Example policy: emit up to a defined percentage of net LUX performance for a period.

Concept:

`DailyMTCMintBudget = PolicyFunction(NetLUXPerformance)`

This keeps MTC tied to real in-game economic activity.

## Reward Inputs

Accepted data items compete for allocation within the daily budget.

Conceptual model:

`RewardPoints = RarityBase * QualityMult * TierMult * DemandMult * FreshnessMult * DupPenalty`

`MTCReward = (RewardPoints / TotalAcceptedPointsForPeriod) * DailyMTCMintBudget`

Where:

- `RarityBase`: common / rare / YARA-9 category baseline
- `QualityMult`: signal quality or scan execution quality
- `TierMult`: satellite tier weight
- `DemandMult`: current corporate demand priority
- `FreshnessMult`: bonus for under-scanned targets
- `DupPenalty`: reduced payout for near-duplicate submissions

## Validation Before Minting

A redemption event must pass validation checks before MTC issuance:

- valid satellite class and tier
- eligible target context
- non-duplicate or non-exploitive submission
- reward window and cooldown compliance
- anti-spam and anti-loop constraints
- duplicate window evaluation (same target/category/time window)

Rejected events do not mint MTC.

## Anti-Abuse Controls

To avoid inflation and repetitive farming, the system applies:

- duplicate payout decay for repeated low-variance data
- diminishing returns on identical high-frequency scans
- cooldown windows by satellite or target context
- throttled low-value output rewards
- dynamic reward curve adjustments based on activity patterns

Example duplicate payout profile for same target and data class in a short window:

- first valid submission: 100%
- second: 60%
- third and beyond: 30%

## Sink Mechanics (Demand Side)

MTC leaves circulation through utility sinks:

- license purchase and renewal
- upgrade installation and module replacement
- premium service access fees
- infrastructure access tolls
- contract entry costs for strategic operations

Note: paying players in MTC from treasury is circulation. Burn only occurs when MTC is explicitly removed from supply by policy.

These sinks are critical to maintaining economic balance and long-term token relevance.

## Balancing Principles

- Utility-first: every reward should map to meaningful spend options.
- Scarcity-aware: rare intelligence should be hard to farm at scale.
- Progression-safe: newcomers should progress without breaking the economy.
- Policy-driven: reward parameters should be adjustable without redesigning the loop.

## KPI Targets for Prototype Stage

- At least 60% of earned MTC is spent within one demo session.
- At least 3 distinct utility sinks are used by test players.
- Repeated scan farming yields visibly lower marginal rewards.
- Players can explain why MTC is useful after one full loop.
- Reward payouts remain within the configured daily mint budget.

## Future On-Chain Scope (Sui)

Planned smart contract responsibilities:

- register satellite classes and license states
- validate redemption events
- mint MTC on accepted submissions
- enforce access permissions and service gating
- apply policy updates to reward balancing parameters

This allows transparent validation while preserving Macana's gameplay-first design.
