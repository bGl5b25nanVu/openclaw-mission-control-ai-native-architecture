# 17 Relationship Model: Goal / Loop / Run / Exception / Policy

## Core chain
Goal <- Loop <- Run -> Evidence
Run -> Exception
Policy constrains Loop and Run
Human intervenes mainly through Exception and Policy changes

## Semantics
### Goal
Desired outcome.

### Loop
Standing improvement or governance cycle operating against a goal/domain.

### Run
One concrete attempt within a loop.

### Exception
A structured reason why a run or loop needs human attention or cannot safely continue.

### Policy
The allowed action scope and escalation boundaries under which loops and runs operate.

## Design implication
Mission Control should visualize this chain explicitly over time.
