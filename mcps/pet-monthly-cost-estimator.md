# Pet Monthly Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-monthly-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate the monthly financial commitment for pet care based on species, size, and location.

## Description
The Pet Monthly Cost Estimator provides detailed breakdowns of the recurring expenses required to maintain a pet. Using tools like `estimate_food_expenses`, `estimate_maintenance_expenses`, and `estimate_risk_and_leisure_expenses`, you can calculate costs for nutrition, health, hygiene, enrichment, and emergency reserves. The estimates adjust dynamically based on species (Dog, Cat, Small Mammal), size tier (Small, Medium, Large), and geographic economic context (Urban or Rural).


## Available Tools (3)
- **estimate_food_expenses**: Calculate the monthly expenditure required for nutritional upkeep
- **estimate_maintenance_expenses**: Calculate monthly costs for health-related care and hygiene services
- **estimate_risk_and_leisure_expenses**: Calculate costs for pet enrichment and the mandatory emergency veterinary fund


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Monthly Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to feed a large dog in an urban area?"

**🤖 AI Agent:**
> To calculate this, I will use the `estimate_food_expenses` tool with species='Dog', sizeTier='Large', and locationType='Urban'.

---

**👤 You:**
> "Estimate the maintenance costs for a small cat in a rural setting."

**🤖 AI Agent:**
> I will use `estimate_maintenance_expenses` with species='Cat', sizeTier='Small', and locationType='Rural' to provide the health and hygiene breakdown.

---

**👤 You:**
> "What is the emergency fund recommendation for a medium-sized small mammal in the city?"

**🤖 AI Agent:**
> I will call `estimate_risk_and_leisure_expenses` using species='Small Mammal', sizeTier='Medium', and locationType='Urban' to find the recommended reserve.


## ❓ FAQ

**Q: What species are supported?**
The estimator currently supports Dog, Cat, and Small Mammal.

**Q: How does location affect the cost?**
Urban locations typically have higher service premiums for grooming and veterinary care compared to Rural areas.

**Q: Does the size of the pet matter?**
Yes, the size tier (Small, Medium, Large) acts as a multiplier for food consumption and hygiene needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-monthly-cost-estimator](https://vinkius.com/mcp/pet-monthly-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Monthly Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-monthly-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Monthly Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-monthly-cost-estimator": {
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
