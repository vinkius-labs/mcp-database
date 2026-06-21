# Glob Pattern Tester MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glob-pattern-tester)
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


## ❓ FAQ

**Q: Is this the same algorithm git uses?**
Yes. minimatch is the glob engine used by npm itself and follows the same POSIX glob specification that git uses for .gitignore.

**Q: Does it support double-star recursive patterns?**
Yes. The `**` pattern matches any number of directories recursively. For example, `src/**/*.ts` matches files at any depth inside `src/`.

**Q: Can I test negation patterns?**
Yes. Prefix any pattern with `!` to negate it. For example, `!node_modules/**` will NOT match any path inside node_modules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glob-pattern-tester](https://vinkius.com/mcp/glob-pattern-tester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glob Pattern Tester** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `glob-pattern-tester` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glob Pattern Tester** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glob-pattern-tester": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
