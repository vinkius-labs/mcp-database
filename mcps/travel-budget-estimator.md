# Travel Budget Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/travel-budget-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate daily travel costs for global cities based on your travel style and group size.

## Description
The Travel Budget Estimator provides a detailed breakdown of daily expenses for travelers. Using tools like `fetch_city_cost_data`, you can retrieve accommodation ranges, meal costs, and transportation estimates for cities worldwide. The `calculate_personal_daily_budget` tool allows you to personalize your budget by adjusting for travel style (backpendacker, mid-range, or luxury) and the number of travelers in your group. For those planning multi-destination trips, `compare_city_budgets` offers a side-by-side comparison of costs between different urban centers.


## Available Tools (3)
- **fetch_city_cost_data**: Fetch cost data for a specific city
- **compare_city_budgets**: Compare budgets between two cities
- **calculate_personal_daily_budget**: Calculate a daily budget for a trip


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Budget Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated daily cost for a backpacker traveling in London with 1 person?"

**🤖 AI Agent:**
> For a backpacker in London, the estimated daily cost per person is approximately $120. This includes hostel accommodation, budget meals, local transit, and attractions.

---

**👤 You:**
> "Compare the daily travel costs between Paris and New York for a mid-range traveler with 2 people."

**🤖 AI Agent:**
> In Paris, the estimated cost is $210 per person. In New York, it is approximately $285 per person. The primary cost driver in both cities is accommodation.

---

**👤 You:**
> "Show me the meal costs and transportation estimates for Tokyo."

**🤖 AI Agent:**
> In Tokyo, daily meal costs range from $30 (budget) to $150 (high-end). Transportation includes a $15 daily transit pass and an estimated $25 for ride-hailing services.


## ❓ FAQ

**Q: How does the tool calculate accommodation costs?**
The tool calculates accommodation by selecting a type based on your travel style (e.g., hostels for backpackers) and then dividing the total cost of the room or bed among the `numberOfTravelers` provided.

**Q: Can I compare more than two cities?**
The `compare_city_budgets` tool is designed to compare the costs of two specific cities at a time to help you evaluate your options clearly.

**Q: What travel styles are supported?**
The tool supports three distinct travel styles: backpacker, mid-range, and luxury. Each style adjusts meal tiers and accommodation types accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/travel-budget-estimator](https://vinkius.com/mcp/travel-budget-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Budget Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-budget-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Budget Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-budget-estimator": {
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
