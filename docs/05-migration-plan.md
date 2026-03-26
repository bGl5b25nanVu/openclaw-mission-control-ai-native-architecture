# 05 Migration Plan

## Phase 1: Semantic migration
Keep current product structures but reinterpret them:
- board group as domain
- board as loop
- task as run

## Phase 2: Dashboard migration
Move dashboard from passive reporting to loop-centric control plane:
- active loops
- exceptions queue
- goal drift
- control actions

## Phase 3: Policy and exception objects
Introduce explicit policy / exception / run lifecycle concepts.

## Phase 4: Autonomy tuning
System should increasingly auto-run routine loops and only escalate genuine exceptions.

## Non-goal
Do not rewrite the whole product in one pass. Preserve operational continuity while changing semantics and control logic incrementally.
