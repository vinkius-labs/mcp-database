# Festival Group Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/festival-group-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Centralized logistics coordinator for managing group itineraries, expenses, and shared resources during music festivals.

## Description
Manage every detail of your festival trip with a single coordinator. This MCP connects your AI agent to essential logistics tools like `plan_itinerary` for scheduling meeting points, `manage_shifts` for assigning duties, `track_expenses` for splitting costs, and `allocate_resources` for distributing tickets or lodging. It ensures your group stays synchronized from arrival to departure.


## Available Tools (5)
- **allocate_resources**: Distributes physical assets like tickets, transport seats, or lodging spots
- **get_group_status**: Provides a high-level overview of the group's current logistics
- **manage_shifts**: Assigns and tracks responsibilities within the group
- **plan_itinerary**: Coordinates the group's schedule by aligning meeting points and time slots
- **track_expenses**: Records shared costs to ensure fair financial distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Festival Group Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan an itinerary for group 'fest-2024' on July 15th with meeting points at 'Main Stage' and 'Food Court'."

**🤖 AI Agent:**
> The itinerary for July 15th is set: 12:00 PM at Main Stage for the opening ceremony, and 3:00 PM at Food Court for lunch.

---

**👤 You:**
> "Assign a food duty shift to Alex from 2:00 PM to 4:00 PM for group 'fest-2024'."

**🤖 AI Agent:**
> Shift assigned: Food duty for Alex is scheduled from 2:00 PM to 4:00 PM.

---

**👤 You:**
> "Record a $50 expense for 'Dinner' paid by Sam, to be split among Sam, Jo, and Bo for group 'fest-2024'."

**🤖 AI Agent:**
> Expense recorded: $50 for Dinner. Individual shares are $16.67 for Sam, Jo, and Bo.


## ❓ FAQ

**Q: How can I see the current group spending?**
You can use the `get_group_status` tool to receive a snapshot of total spending and group logistics.

**Q: Can I assign specific tasks to group members?**
Yes, the `manage_shifts` tool allows you to assign responsibilities like food duty or gear security to specific members.

**Q: How do we split the cost of a shared taxi?**
Use the `track_expenses` tool to record the total amount and list all members who should share the cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/festival-group-planner](https://vinkius.com/en/ai-agent-connect/festival-group-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Festival Group Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `festival-group-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Festival Group Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "festival-group-planner": {
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
