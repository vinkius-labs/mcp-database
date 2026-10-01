# Garden Material Delivery Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-material-delivery-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Distributes bulk material costs and delivery fees across multiple projects.

## Description
This MCP server provides an allocation engine to split bulk material costs and fixed delivery fees across various projects. It uses material quantities and project weightings to ensure proportional distribution. Use `calculate_material_distribution` to partition costs, `calculate_taxed_allocations` to apply project-specific taxes, `get_delivery_efficiency_ratio` to analyze delivery overhead, and `summarize_project_totals` for accounting summaries.


## Available Tools (4)
- **calculate_taxed_allocations**: Applies specific tax rates to the previously distributed material costs
- **get_delivery_efficiency_ratio**: Measures the impact of the delivery fee on the overall material cost
- **summarize_project_totals**: Aggregates all calculated costs into a high-level summary for accounting
- **calculate_material_distribution**: Determines how much of the total material cost and the delivery fee should be assigned to each project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Material Delivery Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a $500 material cost and $50 delivery fee between Project A (10 units) and Project B (30 units)."

**🤖 AI Agent:**
> Project A is allocated $125.00 for materials and $12.50 for delivery. Project B is allocated $375.00 for materials and $37.50 for delivery.

---

**👤 You:**
> "Calculate the total summary for Project A with a material cost of $100 and a tax rate of 5%."

**🤖 AI Agent:**
> The final total cost for Project A is $105.00.

---

**👤 You:**
> "What is the delivery impact for a $1000 material order with a $100 delivery fee?"

**🤖 AI Agent:**
> The delivery impact is 10%.


## ❓ FAQ

**Q: How are delivery fees distributed?**
Delivery fees are distributed proportionally based on the material quantity assigned to each project.

**Q: Can I apply different tax rates to different projects?**
Yes, you can use `calculate_taxed_allocations` to apply specific tax rates to each project's material cost.

**Q: What is the purpose of the efficiency ratio?**
The `get_delivery_efficiency_ratio` tool helps you understand the financial impact of the delivery fee relative to the total material cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-material-delivery-splitter](https://vinkius.com/en/ai-agent-connect/garden-material-delivery-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Material Delivery Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-material-delivery-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Material Delivery Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-material-delivery-splitter": {
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
