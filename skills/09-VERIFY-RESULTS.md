# Skill 09: Verify Results

## Goal

Do not treat an agent statement such as "done" as sufficient proof that an external task actually happened.

## Use acceptance criteria

Before a task starts, define what success looks like.

Example:

Task: Create a test CRM note.

Acceptance criteria:

- the correct test contact was used
- the note text matches the requested text
- the note appears in the CRM after the action
- the result can be read back independently

Use `templates/TASK-ACCEPTANCE.md` for repeatable checks.

## Verification pattern

1. define expected state
2. run the task
3. inspect the destination system or output
4. compare actual state with expected state
5. mark the task accepted only when they match

## Functional acceptance

Run one test where the agent claims success but the destination state is intentionally wrong or incomplete. Your verification step should catch the mismatch.
