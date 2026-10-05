# Wedding Registry Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wedding-registry-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Manage and optimize your wedding gift registry budget.

## Description
This MCP server helps couples manage the complexity of wedding gift registries. It balances desired items against expected guest contributions using advanced allocation logic. Use `calculate_registry_feasibility` to check if your list is realistic, `optimize_item_allocation` to find the best sequence of requests, `simulate_contribution_scenarios` to predict outcomes based on guest patterns, and `get_item_priority_score` to rank item importance.


## Available Tools (4)
- **calculate_registry_feasibility**: Determines if the current list of desired items is realistic given the expected total guest contribution
- **get_item_priority_score**: Calculates a single numerical score for an item to help rank its importance
- **optimize_item_allocation**: Suggests the best sequence of items to request to maximize value for the couple
- **simulate_contribution_scenarios**: Predicts the outcome of different guest contribution styles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Registry Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my registry feasible with a $2000 budget?"

**🤖 AI Agent:**
> The registry is feasible. Your high-priority items are covered, with a remaining surplus of $350.

---

**👤 You:**
> "What is the best way to order my items for a $1500 budget?"

**🤖 AI Agent:**
> To maximize value, you should prioritize the Toaster, Blender, and Coffee Maker, which will be fully funded.

---

**👤 You:**
> "What happens if most guests give small amounts?"

**🤖 AI Agent:**
> With a 'many_small' pattern, there is an 85% probability of completing your low-priced items like the cutlery set and towels.


## ❓ FAQ

**Q: How do I know if my registry is realistic?**
You can use the `calculate_registry_feasibility` tool to compare your desired items against the expected total guest contribution.

**Q: Can I predict how guests will contribute?**
Yes, the `simulate_contribution_scenarios` tool allows you to predict outcomes for different patterns, such as many small gifts versus a few large gifts.

**Q: How are items prioritized?**
Items are ranked using `get_item_priority_score`, which considers price, priority level, and duplicate need to determine the best allocation order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wedding-registry-budget-planner](https://vinkius.com/en/ai-agent-connect/wedding-registry-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Registry Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-registry-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Registry Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-registry-budget-planner": {
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
