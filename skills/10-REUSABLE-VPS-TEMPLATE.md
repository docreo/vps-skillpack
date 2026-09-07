# Skill 10: Reusable VPS Template

## Goal

Turn the accepted build into a repeatable deployment pattern without copying account specific data.

## Capture the reusable pieces

Document:

- VPS size and operating system class
- installation sequence
- Hermes version or release channel used
- required profile names and purposes
- model selection process
- Kanban workflow
- connector categories
- scheduled job categories
- acceptance tests
- backup or snapshot method supplied by your VPS provider

## Do not put account specific values in the template

Use placeholders for:

- provider accounts
- API credentials
- domains
- phone numbers
- customer records
- private URLs
- organization identifiers

## Clone test

Use the template to build a second clean test environment.

The template passes when the second environment can reach the same functional milestones without inheriting data from the first environment.
