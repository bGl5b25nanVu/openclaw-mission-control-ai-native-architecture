# 08 Control Plane MVP

## Goal
Define the minimum viable AI-native dashboard/control plane that should be implemented before broader autonomy features.

## MVP modules
### 1. Goal Drift
- target vs actual
- variance level
- linked domain / loop
- whether mitigation is already active

### 2. Active Loops
- loop name
- domain
- latest run status
- last evidence time
- next expected action

### 3. Exceptions Requiring Human
- blocked by approval
- repeated failed runs
- policy conflict
- missing external dependency
- high-risk external action

### 4. Agent Efficiency
- effective runs
- stalled runs
- repeated failures
- evidence-backed completion rate

## Explicit non-goals for MVP
- full policy editor
- automatic loop generation
- predictive planning across all domains
- complex simulation views

## Launch criteria
- each MVP module has data source mapping
- each MVP module has fallback behavior when data is incomplete
- at least one actionable drill-down exists per module
