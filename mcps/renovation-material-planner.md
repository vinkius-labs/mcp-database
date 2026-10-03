# Renovation Material Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renovation-material-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate material orders, package counts, and delivery deadlines for renovation projects.

## Description
This MCP server provides precise tools for managing renovation material procurement. It calculates the exact number of packages required based on surface area, coverage rates, and waste factors. Use `get_material_requirements` to determine order quantities and leftover amounts, `calculate_delivery_schedule` to find the latest order-by dates, and `get_project_material_summary` for a complete overview of procurement needs including status and deadlines.


## Available Tools (4)
- **calculate_delivery_schedule**: Determines the deadline for placing an order to meet a specific project start date
- **get_material_requirements**: Determines the exact amount of material that needs to be purchased for a specific surface
- **get_project_material_summary**: Provides a high-level overview of the material procurement needs for a single material type
- **validate_material_availability**: Checks if current inventory is sufficient for a proposed plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renovation Material Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to paint a 50m2 wall. The paint covers 10m2 per liter, I need 10% extra for waste, and it comes in 5L buckets. I have 2L in stock. How many buckets should I buy?"

**🤖 AI Agent:**
> You need to order 1 bucket (5L).

---

**👤 You:**
> "When should I order tiles if the project starts on 2024-10-15 and the delivery takes 7 days?"

**🤖 AI Agent:**
> You must place the order by 2024-10-08.

---

**👤 You:**
> "Give me a summary for 100m2 of flooring. Coverage is 2m2 per unit, 5% waste, 10m2 per package, 0 inventory, and 5 days lead time for a start on 2024-12-01."

**🤖 AI Agent:**
> Material: Flooring, Packages to Order: 6, Order-By Date: 2024-11-26, Status: Action Required.


## ❓ FAQ

**Q: How does the tool calculate the number of packages to order?**
The `get_material_requirements` tool calculates the total quantity needed (including waste) and divides it by the package size, rounding up to the nearest whole number.

**Q: Can I check if my current stock is enough for a project?**
Yes, use the `validate_material_availability` tool to compare your required quantity against your current inventory level.

**Q: How do I know when I must place an order?**
The `calculate_delivery_schedule` tool determines the order-by date by subtracting the lead time from your planned project start date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renovation-material-planner](https://vinkius.com/en/ai-agent-connect/renovation-material-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renovation Material Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renovation-material-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renovation Material Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renovation-material-planner": {
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
