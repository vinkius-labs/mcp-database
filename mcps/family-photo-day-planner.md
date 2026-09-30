# Family Photo Day Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-photo-day-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate photography logistics, outfits, travel, and budgets.

## Description
A specialized coordination engine for managing the complex logistics of family photography sessions. This MCP connects AI agents to your photography plan, allowing them to manage the day's flow. Use `get_daily_schedule` to view the chronological timeline, `get_outfit_plan` to manage clothing transitions, and `validate_travel_feasibility` to ensure group movement stays on track. It also handles child-friendly break scheduling via `get_child_care_needs` and print budget tracking with `calculate_budget_status`.


## Available Tools (5)
- **calculate_budget_status**: Checks the remaining funds available for printing based on the current spend and the original limit
- **get_child_care_needs**: Identifies the scheduled breaks and rest periods specifically designed for children
- **get_daily_schedule**: Retrieves the full chronological sequence of events for the planned photography day
- **get_outfit_plan**: Provides the details of what everyone should be wearing during specific segments of the day
- **validate_travel_feasibility**: Checks if the time allocated between two locations is sufficient for the group size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Photo Day Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the schedule for 2024-06-15?"

**🤖 AI Agent:**
> The schedule for June 15th, 2024 includes a photo block at 10:00 AM, an outfit change at 11:30 AM, and a travel window at 12:30 PM.

---

**👤 You:**
> "What should the kids wear for the first photo block?"

**🤖 AI Agent:**
> For the first photo block, the children should wear the blue linen outfits and white sandals.

---

**👤 You:**
> "Is there enough time to travel from the Park to the Studio with 5 people in 30 minutes?"

**🤖 AI Agent:**
> No, the estimated minimum travel time for a group of 5 from the Park to the Studio is 45 minutes.


## ❓ FAQ

**Q: How can I see the full schedule for the day?**
You can use the `get_daily_schedule` tool by providing the specific date of the photo session.

**Q: Can I check if we have enough time to move between locations?**
Yes, the `validate_travel_feasibility` tool checks if the allocated time is sufficient for your group size and locations.

**Q: How do I manage the printing budget?**
Use the `calculate_budget_status` tool to compare your initial budget against current spending to see your remaining balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-photo-day-planner](https://vinkius.com/en/ai-agent-connect/family-photo-day-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Photo Day Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-photo-day-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Photo Day Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-photo-day-planner": {
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
