# Skill 07: Optional GHL Integration

## Goal

Connect a Hermes specialist to GoHighLevel, also known as HighLevel, for a bounded business workflow.

Skip this skill if you do not use GHL.

## Choose one first workflow

Good first tests include:

- read a contact record
- read an opportunity or pipeline state
- create a test note
- update a disposable test record
- create a test task

Do not begin with a complex automated campaign. Prove the smallest useful business action first.

## Integration choices

Depending on your setup, you may connect GHL through:

- HighLevel API or OAuth
- an MCP server
- a supported integration platform
- your own middleware

Use the current HighLevel developer documentation for the method you select.

## Functional acceptance

A designated profile should be able to:

1. receive a CRM task
2. read the expected GHL state
3. perform one test change
4. read GHL again
5. show that the expected change actually exists

That read back step is important because a successful API response is not the same thing as a successful business outcome.
