# Glob Pattern Tester MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glob-pattern-tester)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/glob-pattern-tester-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/glob-pattern-tester-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Test whether a file path matches a glob pattern using the same algorithm used by npm and git. 130M+ weekly downloads.

## Description
When a DevOps agent writes .gitignore rules or CI pipeline includes, it cannot guess whether `src/**/*.ts` matches `src/utils/helper.ts`. This MCP provides the definitive answer.

### The Superpowers

- **Exact Match:** Uses minimatch, the same engine behind npm, to evaluate glob patterns deterministically.
- **All Patterns:** Supports `*`, `**`, `?`, `[abc]`, `{a,b}`, and negation `!`.


## Available Tools
- **test_glob**: gitignore rules, CI include/exclude patterns, or deploy filters. Pass the glob pattern (e.g. "src/**/*.ts") and the file path to test (e.g. "src/utils/helper.ts"). The engine returns a boolean match result using the exact same algorithm used by npm and git.

Tests whether a file path matches a glob pattern using minimatch (130M+ weekly downloads). Essential for .gitignore, CI pipeline, and deploy rule validation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glob Pattern Tester** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Does the pattern src/**/*.ts match the file src/utils/helper.ts?"

**🤖 AI Agent:**
> Glob Match Result: matches = true

---

**👤 You:**
> "Check if *.json matches package.json in the root."

**🤖 AI Agent:**
> Glob Match Result: matches = true

---

**👤 You:**
> "Will !dist/** exclude the file dist/bundle.js?"

**🤖 AI Agent:**
> Glob Match Result: matches = false (negated)


## Installation & Usage

To install and use the **Glob Pattern Tester** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glob-pattern-tester](https://vinkius.com/mcp/glob-pattern-tester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
