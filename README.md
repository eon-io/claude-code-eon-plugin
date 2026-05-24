# Eon Claude Code Plugin

Connect Claude Code to Eon via this plugin. Bundles the Eon MCP server and guided cloud onboarding skills into a single installable package.

## Capabilities

- **Eon MCP server** — 27 tools for multi-cloud backup, recovery, inventory, source account management, backup policies, snapshot browsing, restore jobs, GCP organization/folder onboarding, and resource discovery.
- **GCP onboarding skill** — step-by-step guided workflow to connect GCP organizations, folders, and individual projects to Eon.

## Installation

Run inside Claude Code:

```
/plugin install eon@eon-service
```

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| GCP Onboarding | `/eon:gcp-onboarding` | Guide users through connecting GCP cloud accounts (orgs, folders, or individual projects) to the Eon platform. |

## MCP Server

The plugin connects to `https://mcp.eon.io/mcp` via HTTP. Authentication is handled by the Eon platform.

## Local Development

```bash
claude --plugin-dir .
```

Run `/reload-plugins` inside Claude Code after making local edits.

## Links

- [Eon Platform](https://eon.io)
- [Documentation](https://docs.eon.io)

## License

Licensed under the [Apache License, Version 2.0](LICENSE). See [NOTICE](NOTICE) for attribution and the scope of the license — the Eon service, API, and trademarks are not covered.
