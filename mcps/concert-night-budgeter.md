# Concert Night Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/concert-night-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan and split all expenses for your next concert trip.

## Description
Manage every aspect of your concert outing with precision. This MCP server provides tools to calculate individual budgets, aggregate logistics costs like transport and parking, and handle group expense splits. Use `summarize_event_budget` to see the grand total for the whole group, or `calculate_group_split` to divide shared costs like lodging or ride-shares among friends.


## Available Tools (4)
- **calculate_group_split**: Calculates how much each person owes when a group expense is paid by a single person
- **calculate_individual_total**: Determines how much a single person needs to budget for the entire night
- **estimate_logistics_cost**: Aggregates all movement-related expenses to understand the cost of reaching the venue
- **summarize_event_budget**: Provides a high-level overview of the entire night's planned spending for the whole group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concert Night Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost me for a concert if the ticket is $100, fees are $15, and I plan to spend $40 on food and $25 on a t-shirt?"

**🤖 AI Agent:**
> Your total budget for the concert is $180.

---

**👤 You:**
> "We spent $60 on a taxi for 3 people. How much does each person owe if we split it equally?"

**🤖 AI Agent:**
> Each person owes $20.

---

**👤 You:**
> "What are my total logistics costs if the train costs $30 and parking is $15?"

**🤖 AI Agent:**
> Your total logistics cost is $45.


## ❓ FAQ

**Q: How do I split a shared ride-share cost?**
You can use the `calculate_group_split` tool to divide the total ride-share amount among all participants using either an equal or weighted split.

**Q: Can I include food and merchandise in my budget?**
Yes, the `calculate_individual_total` tool allows you to include estimated spending on food and merchandise to get a complete personal budget.

**Q: How do I see the total cost for the whole group?**
Use the `summarize_event_budget` tool to get a high-level overview, including the grand total and the average cost per person.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/concert-night-budgeter](https://vinkius.com/en/ai-agent-connect/concert-night-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concert Night Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concert-night-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concert Night Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concert-night-budgeter": {
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
