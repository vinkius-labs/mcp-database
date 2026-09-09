# Consolidating Settlement Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/consolidating-settlement-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates primary and secondary settlement of mine tailings using Terzaghi theory.

## Description
This MCP server provides specialized geotechnical tools to model the settlement behavior of mine tailings. It implements Terzaghi's consolidation theory to calculate primary consolidation magnitude and progress, and accounts for secondary compression (creep) caused by particle rearrangement. Engineers can use `get_primary_settlement` to determine initial settlement, `get_secondary_compression` for long-term creep, `get_consolidation_rate` to predict settlement velocity, and `get_settlement_timeline` to generate a complete settlement history over time.


## Available Tools (4)
- **get_primary_settlement**: Calculates the total magnitude and progress of primary consolidation at a specific point in time
- **get_secondary_compression**: Calculates the settlement caused by particle rearrangement (creep) after primary consolidation is finished
- **get_settlement_timeline**: Provides a high-level summary of the total settlement over a series of time intervals
- **get_consolidation_rate**: Determines the velocity of settlement at a specific time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Consolidating Settlement Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the primary settlement for a tailings layer with specific properties after 100 days."

**🤖 AI Agent:**
> The primary consolidation magnitude is 0.45 meters with a degree of consolidation of 85%.

---

**👤 You:**
> "What is the total settlement including secondary compression after the primary phase is done?"

**🤖 AI Agent:**
> The total cumulative settlement is 0.52 meters, consisting of 0.45 meters from primary consolidation and 0.07 meters from secondary compression.

---

**👤 You:**
> "Generate a settlement timeline for the next 500 days."

**🤖 AI Agent:**
> The settlement timeline shows a rapid primary phase reaching 0.45m by day 150, followed by a slow secondary creep phase reaching 0.52m by day 500.


## ❓ FAQ

**Q: How does this model handle secondary compression?**
The model uses the `get_secondary_compression` tool to calculate settlement caused by particle rearrangement (creep) that occurs after the primary consolidation phase is complete.

**Q: Can I predict the rate of settlement for stability analysis?**
Yes, you can use the `get_consolidation_rate` tool to determine the settlement velocity at any specific time, which is essential for predicting near-term stability.

**Q: What inputs are required for primary consolidation?**
To use `get_primary_settlement`, you need to provide tailings properties (compressibility, void ratio, thickness, permeability), loading history (applied stress and preconsolidation pressure), the elapsed time, and the drainage path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/consolidating-settlement-model](https://vinkius.com/ai-agent-connect/consolidating-settlement-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Consolidating Settlement Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `consolidating-settlement-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Consolidating Settlement Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "consolidating-settlement-model": {
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
