# MVP Scan Mechanic v1

## Scope

This MVP defines the simplest playable loop for the first web prototype.

Loop:

`Get Tier 1 -> Scan -> Receive Data Item -> Redeem -> Gain Standing and Reward`

## Player States

- `new`: no standing history
- `active`: has completed at least one successful redemption
- `trusted`: high standing tier

## Tier 1 Access Rules

- Tier 1 units are fabricated by Macana from game resources.
- Public distribution is quota-based and refreshes every 24h.
- Suggested quota by standing tier:
  - low: 5
  - medium: 10
  - high: 15
- Optional anti-hoarding: withdrawal cooldown per unit.

## Scan Inputs

- satellite tier
- target body type
- scan duration
- interruption flag (combat/disruption)
- random variance

## Scan Outputs

- `failed`: no data (satellite lost or interrupted)
- `common_data`
- `rare_data`
- `yara_signature_fragment`

Each successful output mints a `Data Item` with metadata:

- `data_id`
- `source_target_id`
- `rarity`
- `quality_score`
- `created_at`
- `owner_player_id`

## Redemption Validation

The MCC checks:

- item ownership
- item integrity and age window
- target validity
- duplicate window status

Duplicate window behavior example:

- first valid item: 100% payout weight
- second similar item in window: 60%
- third and later: 30%

## Reward Model (Prototype)

Budget policy:

- `DailyMTCMintBudget` is configured from treasury logic linked to LUX performance.

Per-item points:

`RewardPoints = RarityBase * QualityMult * TierMult * DemandMult * DupPenalty`

Payout:

`MTCReward = (RewardPoints / TotalRewardPointsForPeriod) * DailyMTCMintBudget`

## Standing Model (Prototype)

- successful redemption grants standing
- failed scans grant no standing
- standing unlocks higher Tier 1 daily quota and price improvements

## Out of Scope for MVP

- full Tier 3 persistence and heat systems
- on-chain contract integration
- cross-station macro economy balancing

## Success Metrics

- compressed demo loop completion in about 3 minutes
- in-world full cycle timing measured separately (acquire, travel, scan, return, redeem)
- reward and standing feedback is understood without explanation
- duplicate payout penalty is visible in UI
- budget cap is not exceeded in simulation
