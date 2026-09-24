# Transport Leg Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/transport-leg-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates the cumulative cost of a sequence of logistical transport segments.

## Description
This MCP server provides tools to manage and analyze logistical transport chains. It allows AI agents to calculate the total fare of multiple segments, validate leg data for completeness, count the number of transport segments, and identify the most expensive leg in a sequence using tools like `get_total_fare`, `validate_leg_data`, `get_leg_count`, and `find_highest_cost_leg`.


## Available Tools (4)
- **find_highest_cost_leg**: 
- **get_leg_count**: 
- **get_total_fare**: 
- **validate_leg_data**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transport Leg Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total fare for these legs: leg1 with 100, leg2 with 250, and leg3 with 50?"

**🤖 AI Agent:**
> The total fare for the provided transport legs is 400.

---

**👤 You:**
> "How many transport segments are in this list: leg_a (50), leg_b (75), leg_c (30)?"

**🤖 AI Agent:**
> There are 3 transport segments in the sequence.

---

**👤 You:**
> "Which leg is the most expensive: leg_x (10), leg_y (500), leg_z (200)?"

**🤖 AI Agent:**
> The most expensive leg is leg_y with a fare of 500.


## ❓ FAQ

**Q: How do I calculate the total cost of my shipment?**
You can use the `get_total_fare` tool by providing an array of transport legs, each containing its fare.

**Q: Can I verify if my transport data is valid?**
Yes, the `validate_leg_data` tool checks if your transport legs have valid identifiers and non-negative fares.

**Q: How can I find the most expensive part of my journey?**
Use the `find_highest_cost_leg` tool to identify the specific segment with the highest fare in your sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/transport-leg-total](https://vinkius.com/en/ai-agent-connect/transport-leg-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transport Leg Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transport-leg-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transport Leg Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transport-leg-total": {
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
