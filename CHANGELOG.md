# Changelog

All notable changes to this plugin are recorded here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.1] - 2026-10-26

### Changed

- claude.ai: find ZeroMark in Claude's directory first. Paste the server URL only if it is not listed.
- Say "taste in X". The install section includes the agent setup line and the eleven-tool check.

## [1.1.0] - 2026-10-25

### Added

- `get_taste`: what the reader decided, one save at a time (kept and let go per field and per voice, what they let go lately, and the claims their notes dropped, with dates). Nothing a model inferred; it says when there are too few decisions to call it taste.
- `get_map`: the Map's fields with the reader's keep rate, the saves in different fields that share rare ideas, and the notes they pinned together.
- `get_podcast`: the latest saves podcast as text, with a link to listen.
- Every save says who decided it (`decided.by`): only the reader's own Done and Let go count as taste.

### Changed

- The skill leads with the reader's decisions, says how many an answer rests on, and never recommends back what they let go without saying so.
- `weekly_question` is described as a suggestion: the reader decides.
- The README opens with a line to paste into your agent so it sets the connector up for you ("Set up ZeroMark for me by following https://www.zeromark.io/docs/connector/agent-setup.md"), and ends the install with a check: the eleven tools your assistant should list.
- README, banner and descriptions say what the connector is for: other connectors give your AI what you saved; ZeroMark gives it what you decided.

## [1.0.0] - 2026-10-25

### Added

- The `zeromark` plugin, connecting Claude Code to `https://www.zeromark.io/api/mcp` with OAuth sign-in.
- Eight read-only tools: `library_overview`, `search_saves`, `get_save`, `list_by_stage`, `get_memory`, `weekly_question`, `search` and `fetch`.
- The `zeromark-library` skill, which tells Claude which tool fits which question and how to cite saves.
- An MCP Registry entry in `server.json`.

[Unreleased]: https://github.com/asheus/zeromark-plugins/compare/v1.1.1...HEAD
[1.1.1]: https://github.com/asheus/zeromark-plugins/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/asheus/zeromark-plugins/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/asheus/zeromark-plugins/releases/tag/v1.0.0
