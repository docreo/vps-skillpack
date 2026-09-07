# Skill 05: Multi Agent Profiles

## Goal

Split work across separate Hermes profiles so each profile can have a clear operating role.

## Create starter profiles

Example:

```bash
hermes profile create research
hermes profile create builder
hermes profile create content
hermes profile create crm-ops
```

Hermes supports multiple isolated profiles, each with its own configuration, sessions, skills, and home directory.

## Suggested starter roles

### Research

Collects information, compares sources, and returns structured findings.

### Builder

Handles implementation work such as code, configuration, or file generation.

### Content

Turns approved information into usable public or internal content.

### CRM Ops

Handles CRM related tasks when a supported business system is connected.

Use `templates/AGENT-PROFILE.md` to define each role.

## Start small

Use one coordinating profile plus one or two specialist profiles before adding more roles.

## Functional acceptance

Create one Kanban task, assign it to a specialist profile, complete the work, and return the result to the board for review.
