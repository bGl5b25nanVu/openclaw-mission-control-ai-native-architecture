# 02 AI-Native Reframe

## Core shift
Replace the dominant question:
- "What objects need to be managed?"

With:
- "What loops must continuously run to move goals forward?"

## AI-native primitives
Recommended first-class primitives:
- Goal
- Metric
- Loop
- Run
- Policy
- Exception
- Evidence
- Approval
- Agent

## Transitional mapping
Without rewriting the entire product immediately:
- Board Group -> Goal Domain / Strategic Domain
- Board -> Loop
- Task -> Run / Iteration / Attempt

This lets the system preserve the current data model while changing its operating semantics.

## Design principle
Tasks should become executable contracts for agents, not just cards for people.
Each run should encode:
- intent
- allowed action scope
- success criteria
- evidence required
- escalation conditions
- retry / fallback logic
