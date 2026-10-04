# School Event Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-event-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate comprehensive costs for school activities, including transport, meals, and clothing.

## Description
This MCP server provides a complete suite of tools for planning school event budgets. It allows AI agents to calculate expected ticket revenue using `get_ticket_revenue`, estimate apparel expenses with `calculate_clothing_costs`, and determine transportation requirements via `estimate_transportation_needs`. It also handles meal planning with `calculate_meal_budget` and provides a final consolidated budget summary using `compile_event_total` that includes contingency buffers. It is designed to help organizers manage variable and fixed costs for any school-related activity.


## Available Tools (5)
- **calculate_meal_budget**: Determines the total food and beverage expenditure
- **calculate_clothing_costs**: Estimates the total expenditure for event apparel
- **compile_event_total**: Aggregates all individual cost categories and applies a contingency buffer
- **estimate_transportation_needs**: Calculates the cost of moving the group via rented vehicles
- **get_ticket_revenue**: Calculates the total expected income from ticket sales


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Event Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to provide 50 students with 2 meals each at $10 per meal?"

**🤖 AI Agent:**
> The total meal cost for 50 students will be $1,000.

---

**👤 You:**
> "Calculate the transport cost for 120 people if each bus holds 40 people and costs $300 to rent."

**🤖 AI Agent:**
> You will need 3 vehicles, and the total transport cost will be $900.

---

**👤 You:**
> "If I sell 100 tickets at $15 each, what is my total revenue?"

**🤖 AI Agent:**
> The total revenue from ticket sales will be $1,500.


## ❓ FAQ

**Q: How can I calculate the total budget including a safety buffer?**
You can use the `compile_event_total` tool, which allows you to specify a `contingencyPercentage` to add as a buffer to your subtotal.

**Q: Can I estimate how many buses I need for a field trip?**
Yes, the `estimate_transportation_needs` tool calculates both the total transport cost and the number of vehicles required based on attendee count and vehicle capacity.

**Q: How do I calculate the income from selling tickets?**
Use the `get_ticket_revenue` tool by providing the ticket price and the total number of attendees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-event-budget-planner](https://vinkius.com/en/ai-agent-connect/school-event-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Event Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-event-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Event Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-event-budget-planner": {
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
