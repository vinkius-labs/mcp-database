# Boolean Truth Table Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boolean-truth-table-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generates exact truth tables and analyzes logical properties of boolean expressions.

## Description
This MCP server provides tools to analyze and evaluate boolean logic. Use `parse_expression` to check the structure and variable count of a logic string, `generate_truth_table` to produce a complete truth table for all input combinations, and `summarize_expression` to identify if a formula is a tautology, contradiction, or contingent.


## Available Tools (3)
- **generate_truth_table**: 
- **parse_expression**: 
- **summarize_expression**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boolean Truth Table Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a truth table for the expression 'A AND B'"

**🤖 AI Agent:**
> | A | B | Result |
|---|---|--------|
| T | T | T      |
| T | F | F      |
| F | T | F      |
| F | F | F      |

---

**👤 You:**
> "Is 'A OR NOT A' a tautology?"

**🤖 AI Agent:**
> Yes, 'A OR NOT A' is a tautology.

---

**👤 You:**
> "How many variables are in 'A AND (B OR C)'?"

**🤖 AI Agent:**
> The expression contains 3 variables: A, B, and C.


## ❓ FAQ

**Q: What can I do with this MCP?**
You can use `generate_truth_table` to see every possible outcome for a boolean expression or `summarize_expression` to find its logical properties.

**Q: How do I define variables?**
Variables are identified as unique alphanumeric characters within your expression string.

**Q: Is there a limit to the expression complexity?**
The `generate_truth_table` tool has built-in limits to prevent excessive computation for expressions with a very high number of variables.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boolean-truth-table-generator](https://vinkius.com/mcp/boolean-truth-table-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Boolean Truth Table Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boolean-truth-table-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Boolean Truth Table Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boolean-truth-table-generator": {
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
