# 10 Data Model Draft

## Transitional rule
Do not require a full schema rewrite immediately.
Use an additive migration path.

## Candidate first-class concepts
### Goal
- id
- name
- scope
- owner
- target metric ids
- target values
- review cadence
- status

### Loop
- id
- goal_id / domain_id
- name
- purpose
- signal inputs
- default cadence
- policy scope
- success criteria
- escalation conditions
- human intervention boundary
- status

### Run
- id
- loop_id
- intent
- hypothesis
- input snapshot
- actions attempted
- evidence collected
- outcome
- next recommendation
- escalation reason
- created_at / completed_at

### Exception
- id
- loop_id
- run_id
- category
- severity
- requires_human
- blocking reason
- recommended action
- resolution state

### Policy
- id
- scope
- allowed actions
- disallowed actions
- approval boundary
- retry boundary
- external impact class

## Mapping to current schema
- board_group -> goal domain
- board -> loop
- task -> run
- approval -> exception/human decision gateway
- activity -> event stream / evidence trail

## Immediate next step
Encode loop/run/exception semantics in UI and task templates before schema changes.
