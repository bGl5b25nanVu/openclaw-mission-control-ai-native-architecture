# 13 Goal Drift Module Spec

## Purpose
Show which goals are drifting away from target and whether the system is already mitigating them.

## Required fields
- goal name
- target
- actual
- variance
- variance trend
- affected domain
- active loop coverage
- latest evidence timestamp
- severity

## Key decisions
- A drifting goal without active loop coverage should rank above one already under mitigation.
- A persistent moderate drift may outrank a single severe but newly detected drift.

## Actions
- inspect linked loops
- open evidence trail
- increase priority
- escalate to human decision
