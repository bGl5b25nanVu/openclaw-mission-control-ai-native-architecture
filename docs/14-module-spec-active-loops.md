# 14 Active Loops Module Spec

## Purpose
Expose what the system is actively trying to improve right now.

## Required fields
- loop name
- linked goal/domain
- latest run status
- last evidence time
- next expected action
- retry count / repeated failure marker
- blocked / not blocked
- human intervention status

## Sorting
Recommended sort order:
1. blocked active loops
2. high-value active loops with stale evidence
3. healthy active loops

## Actions
- inspect latest run
- inspect exception history
- pause loop
- widen / narrow policy scope
- escalate
