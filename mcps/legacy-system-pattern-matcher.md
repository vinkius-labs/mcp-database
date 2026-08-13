# Legacy System Pattern Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legacy-system-pattern-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identifies legacy code patterns and provides deterministic rules for safe interaction.

## Description
This MCP server acts as a diagnostic bridge for AI agents working on aging codebases. It scans for framework-specific signatures, custom ORM patterns, and non-standard directory structures. Once identified, it provides deterministic interaction rules such as `do_not_modernize` or `wrap_dont_replace` to prevent accidental regressions. Use `scan_codebase` to detect patterns, `get_pattern_details` to retrieve specific protection requirements, and `calculate_risk_assessment` to evaluate the danger level of modifying specific files.


## Available Tools (3)
- **calculate_risk_assessment**: 
- **get_pattern_details**: 
- **scan_codebase**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legacy System Pattern Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan the current directory for legacy patterns."

**🤖 AI Agent:**
> I have scanned the codebase. I detected 3 legacy patterns: an AngularJS module in `src/legacy/app.js`, a jQuery AJAX call in `src/legacy/utils.js`, and a custom ORM pattern in `src/db/connection.js`. The legacy density score is 0.45.

---

**👤 You:**
> "What is the risk level of modifying `src/legacy/app.js`?"

**🤖 AI Agent:**
> The risk level for `src/legacy/app.js` is critical. The density score is 0.8, and the `do_not_modernize` rule is active, meaning you should not attempt to rewrite this file.

---

**👤 You:**
> "Get the rules for the pattern found in `src/legacy/utils.js`."

**🤖 AI Agent:**
> The applicable rules for the pattern in `src/legacy/utils.js` are `wrap_dont_replace` and `preserve_api_surface`.


## ❓ FAQ

**Q: How does the tool identify legacy patterns?**
The tool uses deterministic AST and regex pattern matching to identify specific architectural or syntactical markers in the codebase.

**Q: What are the interaction rules?**
The rules include `do_not_modernize` to prevent regressions, `wrap_dont_replace` to mandate adapters, `preserve_api_surface` for stability, and `test_before_changing` for safety verification.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legacy-system-pattern-matcher](https://vinkius.com/mcp/legacy-system-pattern-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legacy System Pattern Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legacy-system-pattern-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legacy System Pattern Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legacy-system-pattern-matcher": {
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
