# Skill 06: Tools and MCP Connections

## Goal

Give Hermes access to external capabilities without making the connector layer the center of the system.

## Current Hermes MCP commands

The current Hermes CLI includes MCP management commands such as:

```bash
hermes mcp
hermes mcp catalog
hermes mcp list
hermes mcp test NAME
```

For supported catalog entries, the current CLI also supports:

```bash
hermes mcp install NAME
```

For a custom server, use the current Hermes documentation for the supported `hermes mcp add` syntax.

## Connection pattern

For each external capability:

1. define the task you want the tool to perform
2. connect only the service needed for that task
3. run a non destructive test
4. confirm Hermes can see the expected tool
5. run one real but reversible task
6. read the result back from the destination system

## Optional integration platforms

You can use direct APIs, MCP servers, native Hermes integrations, or a third party connection platform such as Composio. The public build pattern is the same: connect a tool, test it, and verify the result.

## Functional acceptance

One specialist profile can use one external tool to complete a defined task and you can independently confirm the result.
