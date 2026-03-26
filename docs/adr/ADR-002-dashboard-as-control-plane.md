# ADR-002: Reframe dashboard as AI control plane

## Status
Accepted

## Context
A reporting dashboard is insufficient when AI becomes the primary operator.
Operators need visibility into goal drift, active loops, exceptions, and intervention points.

## Decision
Reframe dashboard around:
- goal drift
- active loops
- exceptions requiring human action
- agent efficiency

## Consequences
### Positive
- aligns UI with AI-native operating model
- reduces passive reporting bias
- makes human intervention more precise

### Negative
- requires stronger data model discipline
- raises expectations for observability and evidence quality

## Follow-up
Define MVP modules and data contracts before implementation.
