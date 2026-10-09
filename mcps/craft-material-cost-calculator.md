# Craft Material Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/craft-material-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total project costs by aggregating material prices.

## Description
This MCP server provides tools to manage crafting project expenditures. Use `get_material_catalog` to view available items and their prices, `validate_project_materials` to ensure your list is complete, and `calculate_total_project_cost` to find the final sum of all materials.


## Available Tools (4)
- **calculate_total_project_cost**: Calculates the final cumulative cost for an entire crafting project
- **validate_project_materials**: Checks if all materials requested for a project are available in the material catalog
- **calculate_material_item_cost**: Calculates the total cost for a single type of material within a project
- **get_material_catalog**: Retrieves the complete list of available materials and their respective unit costs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craft Material Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 5 units of Wood and 2 units of Iron?"

**🤖 AI Agent:**
> The total cost for 5 units of Wood and 2 units of Iron is 45.00.

---

**👤 You:**
> "List all available materials."

**🤖 AI Agent:**
> The available materials are Wood (5.00), Iron (15.00), and Stone (10.00).

---

**👤 You:**
> "How much does 10 units of Stone cost?"

**🤖 AI Agent:**
> 10 units of Stone will cost 100.00.


## ❓ FAQ

**Q: How do I know which materials are available?**
You can use the `get_material_catalog` tool to retrieve the full list of materials and their unit costs.

**Q: Can I calculate the cost for a single material?**
Yes, use `calculate_material_item_cost` to find the cost for a specific material and quantity.

**Q: What happens if a material is missing from the catalog?**
The `validate_project_materials` tool will identify any missing items, and cost calculations will fail if an invalid material is requested.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/craft-material-cost-calculator](https://vinkius.com/en/ai-agent-connect/craft-material-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craft Material Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `craft-material-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craft Material Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craft-material-cost-calculator": {
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
