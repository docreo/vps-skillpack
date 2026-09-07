# Skill 02: Install Hermes Agent

## Goal

Install Hermes Agent and prove that the core runtime works before adding extra services.

## Current public installer

The current NousResearch documentation provides this Linux installer:

```bash
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
```

Reload your shell after installation:

```bash
source ~/.bashrc
```

If your shell is Zsh, reload the matching shell profile instead.

## First launch

Run:

```bash
hermes
```

Use the setup flow to select a model provider that you already use or are authorized to use.

You can inspect available model configuration with:

```bash
hermes model
hermes config
```

## Functional acceptance

A successful baseline should be able to:

1. start Hermes
2. connect to a selected model provider
3. answer a simple test prompt
4. run a basic built in tool that you choose for testing
5. exit and start again without rebuilding the installation

Do not add profiles, MCP servers, or business tools until the basic runtime works.
