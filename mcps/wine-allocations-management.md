# Wine Allocations Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-allocations-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Optimized distribution planning for finite wine inventory across sales channels.

## Description
This MCP server provides a specialized optimization engine for distributing limited wine inventory. It balances margin targets against customer loyalty and historical growth requirements using advanced fairness constraints. Use `get_allocation_plan` to generate optimized distribution plans, `get_channel_performance_forecast` to predict commercial outcomes, `validate_growth_feasibility` to check growth targets, and `get_allocation_rationale` to understand the logic behind specific channel allocations.


## Available Tools (4)
- **get_allocation_plan**: Generates the primary optimized distribution plan for a specific wine product
- **get_allocation_rationale**: Provides a human-readable explanation for why a specific channel received its specific allocation
- **get_channel_performance_forecast**: Predicts the likely commercial outcome of an allocation for a specific channel
- **validate_growth_feasibility**: Checks if a proposed growth target for a channel is realistic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Allocations Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an allocation plan for wine 'CHATEAU-2023' with 5000 units available. Channel A wants 3000 units with loyalty 0.8, and Channel B wants 4000 units with loyalty 0.5. Target margin is 0.25."

**🤖 AI Agent:**
> The optimized plan allocates 3250 units to Channel A and 1750 units to Channel B to satisfy the margin target and fairness constraints.

---

**👤 You:**
> "What is the expected sell-through for 500 units of 'CHATEAU-2023' in the 'Retail' channel?"

**🤖 AI Agent:**
> The expected sell-through for 500 units in the Retail channel is 85%.

---

**👤 You:**
> "Explain why Channel B received 1750 units in the recent allocation plan."

**🤖 AI Agent:**
> Channel B received 1750 units because the fairness constraint ensured a baseline volume was maintained despite its lower loyalty score compared to Channel A.


## ❓ FAQ

**Q: How does the engine decide the allocation for each channel?**
The engine uses `get_allocation_plan` to calculate volumes by weighing channel loyalty scores and margin targets while applying fairness constraints to ensure all channels maintain a baseline presence.

**Q: Can I predict the revenue for a specific channel?**
Yes, you can use `get_channel_performance_forecast` to obtain projected revenue, margin, and expected sell-through for a given volume.

**Q: How can I verify if a growth request is realistic?**
You can use the `validate_growth_feasibility` tool to check if a target growth percentage is achievable based on historical data and current constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-allocations-management](https://vinkius.com/en/ai-agent-connect/wine-allocations-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Allocations Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-allocations-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Allocations Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-allocations-management": {
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
