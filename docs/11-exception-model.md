# 11 Exception Model

## Principle
Humans should mainly enter the system through exception handling, not routine execution.

## Exception categories
- approval_required
- policy_conflict
- missing_external_input
- repeated_failed_runs
- low_quality_evidence
- strategic_conflict
- high_external_impact

## Exception fields
- source goal / loop / run
- severity
- urgency
- recommended human action
- reversible / irreversible
- evidence summary
- retry recommendation

## UI implications
Dashboard should expose an exception queue that is:
- small
- severity-ranked
- directly actionable

## Non-goal
Do not flood humans with low-value alerts. Exception quality matters more than volume.
