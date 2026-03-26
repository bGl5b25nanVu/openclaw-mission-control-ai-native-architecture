# 19 Board Lead Governance Gap

## Core problem
A board lead becoming online does not automatically mean the board can autonomously drive work.
In the live rollout, board leads could:
- read board tasks
- create board-native tasks
- read task comments

But board leads could not freely:
- comment on arbitrary manager-created inbox tasks
- move newly created inbox tasks directly to `in_progress`
- take over generic inbox flow under existing governance rules

## Why this matters
Without solving this layer, Mission Control can create and provision leads but still fail to achieve genuine board-level autonomy.
The system then remains manager-driven in practice, even when the lead is technically online.

## What the rollout proved
### Already working
- board lead onboarding
- board lead provisioning
- board lead first heartbeat / online convergence
- board lead creation of board-native execution tasks

### Still constrained
- status transitions from `inbox -> in_progress`
- commenting on non-lead-created tasks
- broad task takeover rights

## Architectural conclusion
The autonomy bottleneck eventually moves from infrastructure to governance.
After lead bring-up is solved, the next constraint is:

> what a board lead is actually allowed to do inside the board lifecycle.

## Better operating model
Instead of treating manager-created generic tasks as the primary work unit, the rollout suggests a stronger pattern:
1. manager defines KPI, board boundaries, and policy
2. board lead creates board-native execution tasks
3. board lead owns coordination and task shaping
4. manager/patrol bridges only where current governance still blocks state progression

## Why this is better
- respects current policy boundaries
- reduces dependence on generic inbox tasks
- makes board ownership explicit
- aligns board autonomy with actual permissions instead of fighting them

## Design implication
Mission Control should explicitly support the concept of:
- manager-defined goals
- lead-defined execution tasks
- policy-mediated transitions

That is a different model from ordinary project management software.
It is closer to a layered operating system:
- goals at the top
- leads translating goals into executable work
- workers or loops performing execution
- policies constraining state change

## Recommended next step
Codify a dedicated board-lead execution path rather than trying to retrofit full autonomy onto generic manager-created inbox tasks.
