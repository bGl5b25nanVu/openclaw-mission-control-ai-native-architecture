# 20 Autonomy Rollout Plan

## Goal
Turn Mission Control from a task-capable orchestration dashboard into a system where boards increasingly operate as autonomous execution units.

## Rollout philosophy
Do not attempt full autonomy across every board at once.
Use a staged rollout on a small number of strategically important boards, validate runtime behavior, then expand.

## Stage 1 — execution-layer sample boards
Use a small sample set:
- `weekly-bets`
- `daily-execution`
- `product-dev-workflow`

These boards are useful because they sit close to:
- weekly priorities
- day-to-day execution
- reusable product/engineering process

## Stage 2 — board lifecycle convergence
For each sample board, explicitly validate:
1. board exists
2. onboarding started
3. onboarding confirmed
4. board lead provisioned
5. board lead online
6. board lead can create board-native tasks
7. board lead task flow can reach `in_progress`
8. board lead work can reach `review`
9. board lead work can reach `done`

## Stage 3 — governance bridge
Where current governance prevents full lead autonomy, use an intentional bridge:
- manager or patrol advances status under existing rules
- board lead continues execution inside its allowed boundaries

This is a transitional operating mode, not the end state.

## Stage 4 — policy refinement
Once enough evidence exists, decide whether to change governance so board leads can:
- advance their own tasks from inbox to in_progress
- operate with fewer manager bridges
- take over more of the execution lifecycle directly

## Stage 5 — expand board autonomy
Only after the sample boards are stable should autonomy expand to:
- growth boards
- conversion boards
- retention boards
- data / operations boards

## Health metrics that must be tracked during rollout
- onboarding coverage
- confirmed onboarding count
- board lead online count
- lead-created task count
- lead-owned tasks in progress
- review backlog
- approval backlog
- evidence-backed completion rate
- exception queue cleanliness

## Failure modes to watch
- session exists but heartbeat never lands
- lead online but cannot move work
- manager becomes hidden bottleneck
- governance rules silently prevent autonomy
- patrol scores look green while board autonomy is still structurally weak

## End-state definition
The rollout should be considered successful when:
- critical boards are lead-driven rather than manager-pushed
- live feed shows ongoing progress without manual babysitting
- patrol mostly handles exceptions instead of routine orchestration
- KPI progress is increasingly produced by board-native loops rather than direct manager intervention
