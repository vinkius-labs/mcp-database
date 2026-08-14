# Pivot Points Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pivot-points-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis engine for pivot point, support, and resistance levels.

## Description
This MCP server provides a deterministic calculation engine for technical analysis pivot points. It allows AI agents to identify key market equilibrium levels and potential support and resistance zones using multiple mathematical methodologies. By connecting to Vinkius Edge, agents can use tools like `pivot_classic` for standard calculations, `pivot_fibonacci` for ratio-based levels, `pivot_woodie` for close-weighted pivots, `pivot_camarilla` for tight equilibrium levels, and `pivot_demark` for predictive modeling based on open/close relationships.


## Available Tools (5)
- **pivot_camarilla**: Calculates levels using the Camarilla method, which uses the close and the range to find levels near the equilibrium
- **pivot_classic**: Calculates support and resistance levels using the standard Classic pivot point methodology
- **pivot_demark**: Calculates levels using the DeMark method, where the pivot calculation is determined by the relationship between the open and close
- **pivot_fibonacci**: Calculates support and resistance levels using Fibonacci-based mathematical ratios
- **pivot_woodie**: Calculates levels using the Woodie method, which adjusts the pivot calculation to favor the closing price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pivot Points Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the classic pivot points for a period with high 150, low 140, and close 145."

**🤖 AI Agent:**
> The Classic pivot point is 145.0, with R1 at 155.0, S1 at 135.0, R2 at 155.0, and S2 at 135.0.

---

**👤 You:**
> "What are the Fibonacci resistance levels if the high is 100, low is 90, and close is 95?"

**🤖 AI Agent:**
> The Fibonacci pivot is 95.0, R1 is 98.82, and R2 is 100.9, with S1 at 91.18 and S2 at 89.1.

---

**👤 You:**
> "Find the Camarilla levels for high 50, low 40, and close 45."

**🤖 AI Agent:**
> The Camarilla levels are: R3 at 45.91, R2 at 45.75, R1 at 45.41, S1 at 44.59, S2 at 44.25, and S3 at 44.09.


## ❓ FAQ

**Q: What methodologies are supported?**
The server supports Classic, Fibonacci, Woodie, Camarilla, and DeMark pivot point methodologies.

**Q: How do I use the DeMark method?**
To use the DeMark method, you must provide the previous period's open, high, low, and close prices to the `pivot_demark` tool.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pivot-points-calculator](https://vinkius.com/mcp/pivot-points-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pivot Points Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pivot-points-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pivot Points Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pivot-points-calculator": {
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
