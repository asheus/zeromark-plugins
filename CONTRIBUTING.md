# Contributing

Thanks for helping make ZeroMark work better inside Claude.

## What belongs here

This repository holds the Claude Code plugin: its manifest, the MCP server configuration and the `zeromark-library` skill. The connector itself runs on ZeroMark's servers, so a change to what a tool returns is a feature request, not a pull request here.

Good contributions:

- Clearer guidance in `plugins/zeromark/skills/zeromark-library/SKILL.md`.
- Fixes to install steps for a client that changed its settings.
- Typos and broken links.

## Making a change

1. Fork the repository and create a branch.
2. Make your change.
3. Validate it:

   ```bash
   claude plugin validate .
   claude --plugin-dir ./plugins/zeromark
   ```

   In the session, run `/mcp`, sign in, and ask something that should use your change.
4. If you changed anything users will notice, add a line under **Unreleased** in [CHANGELOG.md](CHANGELOG.md).
5. Open a pull request and fill in the template.

## Style

- Plain words, short sentences. Say what the reader can do.
- No em dashes. Use a comma, a colon or a full stop.
- Version numbers follow [Semantic Versioning](https://semver.org). Bump `version` in both `plugins/zeromark/.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json` together.

## Reporting problems

Use the [issue forms](https://github.com/asheus/zeromark-plugins/issues/new/choose). For anything security related, follow [SECURITY.md](SECURITY.md) instead.
