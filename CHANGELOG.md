# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- version list -->

## [0.2.1] - 2025-12-29

### Added
- Test suite with 70 tests covering Obsidian client and all tool handlers
- GitHub Actions CI workflow (Python 3.11-3.13, pyright, pytest)
- Semantic release automation for versioning
- Tool annotations (readOnlyHint, destructiveHint) for 5 tools
- `obsidian_dataview_query` tool for executing Dataview DQL queries
- Windows UTF-8 fix for MCP STDIO communication
- Character encoding fix (`ensure_ascii=False`) for non-ASCII content

### Fixed
- JSONDecodeError on non-JSON HTTP error responses
- Code formatting with ruff (consistent 4-space indentation)
- Removed duplicate API key validation

### Changed
- Upgraded mcp dependency from 1.1.0 to 1.24.0+
- Added ruff and python-semantic-release to dev dependencies

## [0.2.0] - 2024-12-XX (Original Project)

### Added
- Active note operations (get, post, put, patch, delete)
- Periodic notes management (daily, weekly, monthly, quarterly, yearly)
- Command execution tools
- Recent periodic notes and recent changes tools
- Path encoding for Unicode filenames, spaces, emojis

## [0.1.0] - 2024-XX-XX (Original Project)

### Added
- Initial MCP server implementation
- Basic vault file operations (list, get, search, append, patch, put, delete)
- Obsidian Local REST API integration
