# 04 Dashboard as Control Plane

## Dashboard should answer
- Which goals are drifting?
- Which loops are active?
- Which loops are stalled?
- Which exceptions require human action?
- Which agents are producing useful output vs low-value activity?
- What will the system likely do next if no human intervenes?

## Recommended dashboard sections
### 1. Goal Drift
- KPI variance
- trend vs target
- domain impacted
- whether a loop is already handling it

### 2. Active Loops
- loop name
- owning domain
- latest run
- current status
- evidence freshness
- next expected action

### 3. Exceptions Requiring Human
- blocked by approval
- blocked by missing data
- blocked by policy conflict
- blocked by external dependency
- repeated failed runs

### 4. Agent Efficiency
- useful run rate
- repeated failure rate
- stale agent ratio
- evidence-backed completion rate

### 5. Control Surface
- approve
- pause loop
- increase priority
- reassign responsibility
- widen / narrow policy scope
