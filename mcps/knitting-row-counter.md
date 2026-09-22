# Knitting Row Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/knitting-row-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the exact number of rows needed for your knitting projects.

## Description
This MCP server provides essential tools for knitters to manage project dimensions. By providing your target height and row gauge, you can use `get_row_count` to find the total rows required, `validate_gauge_consistency` to ensure your gauge is realistic, `compare_height_targets` to see the difference between two sizes, and `get_project_summary` for a complete vertical overview.


## Available Tools (4)
- **compare_height_targets**: Determines the difference in row counts between two different target heights
- **get_project_summary**: Provides a complete overview of a project's vertical requirements
- **get_row_count**: Calculates the total number of rows needed to reach a target height
- **validate_gauge_consistency**: Checks if the provided row gauge is physically realistic for standard knitting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knitting Row Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many rows do I need for a 10 inch scarf with a gauge of 8 rows per inch?"

**🤖 AI Agent:**
> You will need 80 rows to reach a height of 10 inches.

---

**👤 You:**
> "What is the difference in rows between a 20cm sweater and a 25cm sweater if my gauge is 5 rows per cm?"

**🤖 AI Agent:**
> The difference is 25 rows.

---

**👤 You:**
> "Give me a summary for a project that is 50cm tall with 4 rows per cm."

**🤖 AI Agent:**
> For a 50cm project with 4 rows per cm, you need 200 total rows, and each row is approximately 0.25cm high.


## ❓ FAQ

**Q: How do I use the row counter?**
You can use `get_row_count` by providing the desired height and your row gauge (rows per inch or cm).

**Q: Can I check if my gauge is realistic?**
Yes, use `validate_gauge_consistency` to check if your row gauge falls within standard knitting limits.

**Q: How does the tool handle rounding?**
The tool uses standard mathematical rounding to provide the nearest whole number of rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/knitting-row-counter](https://vinkius.com/en/ai-agent-connect/knitting-row-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knitting Row Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knitting-row-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knitting Row Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knitting-row-counter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
