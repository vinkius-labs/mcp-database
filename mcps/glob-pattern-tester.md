# Glob Pattern Tester MCP Server

Test whether a file path matches a glob pattern using the same algorithm used by npm and git. 130M+ weekly downloads.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/glob-pattern-tester)

## Overview
**Category:** loved-by-devs
**Tools Count:** 1

## Description
When a DevOps agent writes .gitignore rules or CI pipeline includes, it cannot guess whether `src/**/*.ts` matches `src/utils/helper.ts`. This MCP provides the definitive answer.

### The Superpowers

- **Exact Match:** Uses minimatch, the same engine behind npm, to evaluate glob patterns deterministically.
- **All Patterns:** Supports `*`, `**`, `?`, `[abc]`, `{a,b}`, and negation `!`.


## Available Tools
- **test_glob**: gitignore rules, CI include/exclude patterns, or deploy filters. Pass the glob pattern (e.g. "src/**/*.ts") and the file path to test (e.g. "src/utils/helper.ts"). The engine returns a boolean match result using the exact same algorithm used by npm and git.

Tests whether a file path matches a glob pattern using minimatch (130M+ weekly downloads). Essential for .gitignore, CI pipeline, and deploy rule validation


## Installation & Usage

To install and use the **Glob Pattern Tester** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glob-pattern-tester](https://vinkius.com/mcp/glob-pattern-tester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
