# ADR-001: Adopt loop-centric semantics without immediate schema rewrite

## Status
Accepted

## Context
Mission Control already has operational value, but its dominant semantics remain closer to task/project management than AI-native control.
A full schema rewrite would slow progress and risk breaking current operational continuity.

## Decision
Retain the current board-group / board / task storage model initially, but reinterpret semantics as:
- board group -> goal domain
- board -> loop
- task -> run / iteration

## Consequences
### Positive
- preserves continuity
- low migration risk
- allows immediate AI-native framing improvements

### Negative
- semantic mismatch remains visible in UI until later iterations
- some AI-native concepts remain implicit rather than first-class

## Follow-up
Later iterations may introduce explicit loop / run / exception / policy objects.
