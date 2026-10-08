# Home Spa Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-spa-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan spa sessions by calculating product needs, costs, and time feasibility.

## Description
This MCP server provides a complete planning engine for hosting home spa experiences. It allows AI agents to manage product inventory, calculate exact quantities and costs for any number of guests, validate session schedules against time constraints, and ensure all planned activities stay within a specific budget. Use `get_product_catalog` to browse available items, `calculate_session_requirements` to determine how many packages to buy, `validate_time_schedule` to check activity durations, and `check_budget_feasibility` to confirm financial limits.


## Available Tools (4)
- **check_budget_feasibility**: Determines if the planned cost is within the budget limit
- **get_product_catalog**: Retrieves the list of available spa products
- **validate_time_schedule**: Checks if spa activities fit within the available time
- **calculate_session_requirements**: Calculates product quantities and total cost for a session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Spa Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What products are available in the skincare category?"

**🤖 AI Agent:**
> The available skincare products include the Lavender Facial Mask and the Vitamin C Serum.

---

**👤 You:**
> "How much will it cost to host 4 guests with a facial mask using 15ml per person?"

**🤖 AI Agent:**
> For 4 guests, you will need to purchase 1 package of the facial mask, costing a total of $25.00.

---

**👤 You:**
> "Can I fit a 30-minute soak and a 20-minute mask application into a 45-minute window?"

**🤖 AI Agent:**
> No, the total duration of 50 minutes exceeds your available 45 minutes.


## ❓ FAQ

**Q: How does the tool calculate product quantities?**
The `calculate_session_requirements` tool calculates the total amount needed based on guest count and usage per person, then determines how many full packages must be purchased to cover that amount.

**Q: Can I check if my spa activities will fit in my schedule?**
Yes, you can use `validate_time_schedule` to provide your total available minutes and a list of activities to see if the session is feasible.

**Q: How do I know if I am staying within my budget?**
You can use `check_budget_feasibility` by providing the total planned cost and your maximum budget limit to receive a status report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-spa-planner](https://vinkius.com/en/ai-agent-connect/home-spa-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Spa Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-spa-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Spa Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-spa-planner": {
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
