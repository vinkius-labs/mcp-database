# Festival Trip Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/festival-trip-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and manage comprehensive costs for music and arts festival trips.

## Description
Plan your next festival adventure with precision. This MCP server allows AI agents to manage every aspect of a festival trip budget, from individual purchases to shared group costs. Use `get_trip_summary` to see a high-level overview of totals and per-person costs, or `add_expense` to record new items like tickets, lodging, or food. You can also use `list_expenses_by_category` to organize spending and `calculate_individual_share` to determine exactly what each participant owes for shared expenses like rental cars or Airbnbs.


## Available Tools (4)
- **get_trip_summary**: Provides a high-level overview of the entire festival budget
- **calculate_individual_share**: Determines how much a specific person owes based on shared expenses
- **add_expense**: Records a new expense for the trip
- **list_expenses_by_category**: Filters and retrieves expenses belonging to a specific cost type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Festival Trip Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for my festival trip with ID 'trip_123'?"

**🤖 AI Agent:**
> The total cost for trip 'trip_123' is $1,250.00, which averages to $416.67 per person for the 3 participants.

---

**👤 You:**
> "Add a shared expense of $300 for a rental car under the transport category for trip 'trip_123'."

**🤖 AI Agent:**
> The rental car expense has been successfully added to trip 'trip_123'.

---

**👤 You:**
> "How much does participant 'user_456' owe for trip 'trip_123'?"

**🤖 AI Agent:**
> Participant 'user_456' owes a total of $350.00, including their individual expenses and their share of the group costs.


## ❓ FAQ

**Q: How are shared expenses calculated?**
Shared expenses are totaled and then divided equally among all participants in the trip to determine each person's contribution.

**Q: What categories of expenses can I track?**
You can track tickets, lodging, transport, food, merchandise, and fees.

**Q: Can I see a summary of my total spending?**
Yes, by using the `get_trip_summary` tool, you can retrieve the total trip cost, per-person cost, and a breakdown by category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/festival-trip-budgeter](https://vinkius.com/en/ai-agent-connect/festival-trip-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Festival Trip Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `festival-trip-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Festival Trip Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "festival-trip-budgeter": {
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
