# Roadmap: YARA-9 Exploration Network

## Strategic Goal

Deliver a credible vertical slice that proves three things:

1. The exploration loop is understandable and engaging.
2. MTC has clear utility beyond reward accumulation.
3. The system can evolve into on-chain validation on Sui.

## Phase 0 - Foundation (Complete)

- Core concept defined (Macana exploration intelligence economy).
- High-level architecture documented.
- Gameplay loop and token utility direction established.

## Phase 1 - Documentation Lock (Week 1)

Objective: align on a single coherent product narrative.

Deliverables:

- finalized system overview document
- tokenomics framework with anti-abuse logic
- 2-3 minute pitch script
- visual narrative references for satellite, hub, and UI

Success criteria:

- any team member can explain the full loop in under 90 seconds
- all docs use consistent terminology (scan, redeem, validate, spend)

## Phase 2 - Interactive Web Prototype (Weeks 2-3)

Objective: ship a playable simulation of the core loop.

Deliverables:

- web landing with project narrative and value proposition
- interactive flow: Acquire -> Scan -> Retrieve Data Item -> Redeem -> Progress
- standing-based Tier 1 quota panel (5/10/15 per 24h)
- simulated scan outputs and failure events (common, rare, YARA-9, interruption)
- redemption validation with duplicate window penalty states
- MTC reward preview tied to daily budget simulation

Success criteria:

- first-time user completes a compressed demo loop in about 3 minutes
- in-world full cycle target includes travel, scan time, return, and redemption windows
- at least 3 MTC spend actions are demonstrated clearly
- understand the progression without technical explanation

## Phase 3 - Demo Hardening (Week 4)

Objective: prepare a stable, presentable submission.

Deliverables:

- polished UX copy and coherent visual identity
- bug fixes and mobile responsive behavior
- fallback states for scan errors, validation failure, and quota exhaustion
- final presentation build and live walkthrough script
- FAQ with economy and anti-abuse explanations

Success criteria:

- demo runs end-to-end without blockers
- story, mechanics, and economy are clear in a single session

## Phase 4 - Post-Hackathon Technical Expansion (Month 2+)

Objective: evolve prototype into system-ready implementation.

Deliverables:

- backend service for persistent scan and redemption events
- policy engine for reward curve adjustments
- initial Sui smart contract proof-of-concept
- telemetry dashboard for balancing decisions

Success criteria:

- smart contract validates at least one complete redemption flow
- balancing parameters can be changed without app redeploy

## Risks and Mitigation

- Scope overload -> keep first release to one polished loop.
- Token confusion -> emphasize utility sinks in all UI states.
- Balance exploitation -> implement diminishing returns early.
- Presentation drift -> lock final pitch narrative before final week.

## Immediate Next Actions

1. Freeze v1 ruleset (quota, licenses, reward budget, duplicate penalties).
2. Define scan mechanic state map and event table.
3. Build the interactive scan-and-redeem loop before advanced visual polish.
4. Prepare a 10-question stakeholder FAQ and rehearse timing.
