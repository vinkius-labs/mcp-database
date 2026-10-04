# Study Space Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/study-space-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan an optimized study environment by selecting furniture and tools within your physical space and budget constraints.

## Description
This MCP server helps you design the perfect study area. It automates the selection of a complete ergonomic set--including a desk, chair, lighting, and storage--ensuring every item fits within your room's dimensions and stays within your budget. You can also use `find_optimal_configuration` to automatically pick the best furniture combination or `get_available_inventory` to browse specific items. Once you have a selection, use `validate_spatial_fit` to confirm the items fit your floor plan and `calculate_ergonomic_score` to see the quality rating of your setup.


## Available Tools (4)
- **calculate_ergonomic_score**: Evaluates the quality of a configuration based on item prices
- **find_optimal_configuration**: Calculates the best combination of furniture and tools
- **get_available_inventory**: You can filter by category.

Lists all available items across all categories
- **validate_spatial_fit**: Checks if a specific group of items can physically fit into a defined floor area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Study Space Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me a study setup for a $500 budget that fits in a 2m x 2m space."

**🤖 AI Agent:**
> I have found an optimal configuration: a Minimalist Desk ($150), an Ergonomic Task Chair ($200), a LED Desk Lamp ($50), and a Small Bookshelf ($100). The total cost is $500, and all items fit within your 2m x 2m space.

---

**👤 You:**
> "What items are available in the desk category?"

**🤖 AI Agent:**
> The available desks are: Wood Study Desk ($120), Compact Desk ($80), and Executive Desk ($300).

---

**👤 You:**
> "How good is my current furniture selection?"

**🤖 AI Agent:**
> Your current selection has a 'Standard' rating based on the total price of the mandatory items.


## ❓ FAQ

**Q: How do I find the best furniture for my budget?**
You can use the `find_optimal_configuration` tool, which calculates the best combination of mandatory furniture and optional tools based on your specific budget and room dimensions.

**Q: Can I check if my furniture will fit in my room?**
Yes, the `validate_spatial_fit` tool allows you to verify if a specific group of items will physically fit within your available floor width and depth.

**Q: What items are included in a complete set?**
A complete ergonomic set consists of exactly one desk, one chair, one lighting solution, and one storage unit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/study-space-budget-planner](https://vinkius.com/en/ai-agent-connect/study-space-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Study Space Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `study-space-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Study Space Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "study-space-budget-planner": {
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
