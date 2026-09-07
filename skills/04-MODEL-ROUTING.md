# Skill 04: Model Routing

## Goal

Select models based on task fit instead of assuming one model should do everything.

## Configure models

Use the interactive Hermes model command:

```bash
hermes model
```

Review the currently available providers and models in your own environment. Provider catalogs, free tiers, pricing, limits, and model names change over time.

## Build a small test suite

Test at least these task types:

- short factual response
- summarization
- structured JSON output
- tool use
- multi step planning
- coding or shell reasoning if your workflow needs it

Use `templates/MODEL-TEST-MATRIX.csv` to record results.

## Routing pattern

A simple routing strategy is:

1. pick a low cost or local model for routine work
2. use a stronger model when the task needs more reasoning or tool reliability
3. use a specialist model when a task has a specific technical requirement
4. record which model actually produced the accepted result

## Functional acceptance

Choose at least one primary model and one alternate model that both complete your basic task suite successfully.
