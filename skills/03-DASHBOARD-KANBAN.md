# Skill 03: Dashboard and Kanban

## Goal

Create a durable task board that can be used by you and by multiple Hermes profiles.

## Initialize Kanban

Run:

```bash
hermes kanban init
```

## Start the dashboard

Run:

```bash
hermes dashboard --no-open
```

The current Hermes documentation describes the Kanban board as a durable SQLite backed task board shared across Hermes profiles.

## Create a test task

Example:

```bash
hermes kanban create "First VPS test" --body "Return a short host summary and record the result in the task." --priority 1
```

## Functional acceptance

Confirm that you can:

- see the task on the Kanban board
- move or update the task state
- attach a result or comment
- restart the Hermes runtime and still see the task

This proves you have persistent operational state instead of a single temporary chat session.
