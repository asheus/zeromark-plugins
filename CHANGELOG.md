# Changelog

All notable changes to this plugin are recorded here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-10-25

### Added

- The `zeromark` plugin, connecting Claude Code to `https://www.zeromark.io/api/mcp` with OAuth sign-in.
- Eight read-only tools: `library_overview`, `search_saves`, `get_save`, `list_by_stage`, `get_memory`, `weekly_question`, `search` and `fetch`.
- The `zeromark-library` skill, which tells Claude which tool fits which question and how to cite saves.
- An MCP Registry entry in `server.json`.

[Unreleased]: https://github.com/asheus/zeromark-plugins/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/asheus/zeromark-plugins/releases/tag/v1.0.0
