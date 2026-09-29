# Spare Parts Stock Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/spare-parts-stock-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Strategic replenishment and reorder trigger system for critical equipment components.

## Description
Manage inventory risks by connecting your AI agents to critical equipment data. This MCP provides tools to identify immediate reorder needs via `get_reorder_triggers`, generate proactive schedules with `calculate_replenishment_plan`, monitor inventory status using `check_stock_health`, and predict depletion changes with `simulate_usage_impact`.


## Available Tools (4)
- **calculate_replenishment_plan**: Generates a forward-looking schedule of when to order parts
- **check_stock_health**: Provides a high-level diagnostic of the inventory status for a specific part
- **get_reorder_triggers**: Identifies which specific parts currently require an immediate order
- **simulate_usage_impact**: Predicts how a change in the equipment schedule will affect part depletion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spare Parts Stock Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which parts need reordering for equipment EQ-99?"

**🤖 AI Agent:**
> The following parts require immediate orders for EQ-99: Bearing-X (Current: 2, Trigger: 5, Suggested: 10) and Seal-Y (Current: 1, Trigger: 3, Suggested: 5).

---

**👤 You:**
> "Show me the replenishment plan for the next 30 days."

**🤖 AI Agent:**
> The 30-day plan includes ordering 5 units of Gear-Z on 2024-06-15 and 12 units of Bolt-A on 2024-06-20.

---

**👤 You:**
> "What is the stock health for part ID P-102?"

**🤖 AI Agent:**
> Part P-102 is currently in Warning status. There are 12 days of stock remaining, and the risk level is moderate.


## ❓ FAQ

**Q: How do I know which parts need to be ordered immediately?**
You can use the `get_reorder_triggers` tool to identify specific parts that have fallen below their safety stock thresholds.

**Q: Can I plan for future inventory needs?**
Yes, the `calculate_replenishment_plan` tool generates a forward-looking schedule based on a specified number of days.

**Q: How does increased equipment usage affect my stock?**
The `simulate_usage_impact` tool allows you to predict how changes in the equipment schedule will accelerate part depletion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/spare-parts-stock-plan](https://vinkius.com/en/ai-agent-connect/spare-parts-stock-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spare Parts Stock Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spare-parts-stock-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spare Parts Stock Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spare-parts-stock-plan": {
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
