# 18 Board Onboarding Runtime

## Why this document exists
The earlier architecture work defined onboarding as an important step in turning a board into a true agent-native operating unit.
A live Mission Control rollout on the TrueNAS deployment showed that this step is not automatic and must be treated as a first-class runtime lifecycle.

## Key finding
Board creation does **not** automatically complete board onboarding.
The real lifecycle is:
1. create board
2. start onboarding
3. collect onboarding draft / lead-agent draft
4. confirm onboarding
5. provision board lead agent
6. wait for first heartbeat and runtime convergence

## Operational implication
Any architecture that assumes a board is immediately "AI-operable" after creation is incomplete.
A board only becomes a real autonomous unit after:
- onboarding has been started
- onboarding has been confirmed
- a board lead has been provisioned
- the board lead has actually checked in

## Runtime evidence from rollout
Three sample execution boards were used as the first controlled rollout:
- `weekly-bets`
- `daily-execution`
- `product-dev-workflow`

The rollout showed a clear progression:
- before onboarding: boards existed, but no board-level agents existed
- after onboarding start: sessions were created, but work still did not advance automatically
- after onboarding confirm: board lead agent records were created and lead workspaces were rendered
- after first successful heartbeat: board leads became real operating actors

## Architectural lesson
Board onboarding is not a UX accessory.
It is the **boundary between static structure and live autonomous operation**.

## Design consequences
1. Onboarding coverage must be part of system health scoring.
2. Sample boards should be onboarded before broad rollout.
3. Board onboarding should be visible as a lifecycle state, not hidden in setup flows.
4. Board autonomy metrics should distinguish:
   - board exists
   - onboarding started
   - onboarding confirmed
   - lead provisioned
   - lead online

## Recommended principle
A board should be considered autonomous only after the first successful board-lead heartbeat.
