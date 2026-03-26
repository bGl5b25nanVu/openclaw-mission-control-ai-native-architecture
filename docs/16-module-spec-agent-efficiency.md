# 16 Module Spec: Agent Efficiency

## Purpose
Measure whether agents are producing useful motion, not just activity volume.

## Required indicators
- evidence-backed completion rate
- repeated failed run rate
- stale run ratio
- low-value repetition signals
- average time-to-evidence
- active vs idle vs blocked state

## Interpretation
High activity with low evidence is bad.
A quieter agent producing strong evidence can be more valuable than a busy one.

## Actions
- inspect agent run history
- reduce scope
- reassign domain
- pause low-value activity
