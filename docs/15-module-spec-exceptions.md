# 15 Module Spec: Exceptions Requiring Human

## Purpose
Present only the exceptions where human attention adds real value.

## Required fields
- exception type
- source goal/loop/run
- severity
- urgency
- why AI cannot safely continue
- recommended human action
- evidence summary
- reversible / irreversible

## Design rule
This queue should stay small and useful.
If the queue becomes noisy, the exception model is broken.

## Actions
- approve / reject
- reprioritize
- change policy
- defer
- assign owner
