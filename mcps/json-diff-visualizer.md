# JSON Diff Visualizer MCP Server

Generate human-readable visual diffs between two JSON objects — added lines in green, removed in red, unchanged in gray. Like 'git diff' but for JSON structures.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/json-diff-visualizer)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
Your deployment pipeline just changed a config file. You need to review the changes before approving. The deep-diff engine gives you machine-readable change objects — but you need to show the diff to a human for approval.

This MCP generates visual, colorized diffs with `+` and `-` markers — the same format every developer reads in git. But for JSON structures, not file lines.

### The Superpowers

- **Visual Format:** Green `+` for additions, red `-` for removals — instantly scannable by humans.
- **Structural Awareness:** Diffs JSON by structure, not by text lines. Reordered keys don't show as changes.
- **Human Review Ready:** Output designed for Slack messages, PR comments, and approval workflows.
- **Complementary:** Use with deep-diff-engine for programmatic processing, json-diff-visualizer for human review.


## Available Tools
- **diff_json**: Pass two JSON strings and receive both a structural diff (machine-readable) and a visual diff (human-readable with + and - markers). Essential for CI/CD agents comparing config versions, deployment manifests, or database schema snapshots.

Generates structural and visual diffs between two JSON objects. Shows added, removed, and modified fields with exact paths


## Installation & Usage

To install and use the **JSON Diff Visualizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-diff-visualizer](https://vinkius.com/mcp/json-diff-visualizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
