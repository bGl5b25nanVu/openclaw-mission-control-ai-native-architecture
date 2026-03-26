# ADR-003: Humans should primarily enter through exceptions

## Status
Accepted

## Context
AI-native systems lose leverage when humans remain the routine execution engine.
Human attention is the scarcest operating resource.

## Decision
Design the system so humans primarily enter through:
- approvals
- strategic conflicts
- repeated failed loops
- high-risk or external-impact actions

## Consequences
### Positive
- preserves human attention for high-value intervention
- strengthens autonomy defaults
- increases pressure for evidence quality and exception quality

### Negative
- requires better observability
- requires tighter escalation logic

## Follow-up
Define exception schemas, ranking rules, and dashboard presentation.
