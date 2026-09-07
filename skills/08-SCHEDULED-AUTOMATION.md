# Skill 08: Scheduled Automation

## Goal

Prove that useful work can run on schedule without you manually opening a chat.

## Current Hermes cron examples

The current Hermes documentation supports schedule forms such as:

```bash
hermes cron create "every 2h"
hermes cron create "0 9 * * *"
hermes cron create "30m"
```

Use the current CLI help and documentation to add the prompt, target, and delivery options required for your version.

## Start with one useful internal job

Examples:

- daily task summary
- morning research brief
- pipeline status snapshot
- website or service status check
- Kanban triage task

## Functional acceptance

The scheduled job should:

1. fire at the expected time
2. produce an output
3. leave a record you can inspect
4. be easy to pause or remove

Once one scheduled job works reliably, add more only when they have a clear purpose.
