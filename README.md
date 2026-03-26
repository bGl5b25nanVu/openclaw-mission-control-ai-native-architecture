# OpenClaw Mission Control AI-Native Architecture

This repository records the architecture design, operating model, and iteration history for evolving OpenClaw Mission Control from an AI-enhanced management dashboard into an AI-native operating system.

## Current focus
- Reframe Mission Control around goals, loops, runs, exceptions, and policies
- Preserve existing board/group structures while gradually changing semantics
- Turn dashboard into an AI control plane instead of a passive reporting screen
- Record each architecture iteration with explicit rationale and trade-offs

## Documents
- `docs/01-current-state.md`
- `docs/02-ai-native-reframe.md`
- `docs/03-target-operating-model.md`
- `docs/04-dashboard-control-plane.md`
- `docs/05-migration-plan.md`
- `docs/06-iteration-log.md`
- `docs/18-board-onboarding-runtime.md`
- `docs/19-board-lead-governance-gap.md`
- `docs/20-autonomy-rollout-plan.md`

## Design stance
Mission Control should assume:
- AI is the default operator
- Humans define goals, approve exceptions, and resolve strategic conflicts
- System design should optimize for closed loops, evidence, escalation, and goal drift control
