# Eon Claude Code Plugin

Connect Claude Code to Eon via this plugin. Bundles the Eon MCP server and guided cloud onboarding skills into a single installable package.

## Capabilities

- **Eon MCP server** — 27 tools for multi-cloud backup, recovery, inventory, source account management, backup policies, snapshot browsing, restore jobs, GCP organization/folder onboarding, and resource discovery.
- **GCP onboarding skill** — step-by-step guided workflow to connect GCP organizations, folders, and individual projects to Eon.
- **AWS onboarding skill** — step-by-step guided workflow to connect AWS source accounts via the Eon CloudFormation template.
- **Backup policy creation skill** — guided wizard for creating backup policies: pick a policy type, define the resource selector, configure schedules with vaults and retention.

## Installation

Run inside Claude Code:

```
/plugin install eon@eon-service
```

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| GCP Onboarding | `/eon:gcp-onboarding` | Guide users through connecting GCP cloud accounts (orgs, folders, or individual projects) to the Eon platform. |
| AWS Onboarding | `/eon:aws-onboarding` | Guide users through connecting AWS source accounts: deploy the Eon CloudFormation stack, register the role ARN, run discovery. |
| Backup Policy Creation | `/eon:backup-policy-creation` | Guide users through creating a backup policy: type, resource selector, schedules with vaults + retention. |

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
