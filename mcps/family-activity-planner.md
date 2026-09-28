# Family Activity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-activity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize family activities by managing budgets, deadlines, and schedules.

## Description
This MCP server acts as an intelligent planning engine for families. It resolves logistical constraints such as registration deadlines, budget limits, and scheduling conflicts. Use `generate_registration_plan` to create a complete itinerary with payment calendars and equipment checklists. You can also use `validate_activity_feasibility` to check if a new activity fits your current plan, `get_equipment_summary` to consolidate gear lists, and `find_activity_alternates` to discover new options when a preferred activity is unavailable due to constraints.


## Available Tools (4)
- **find_activity_alternates**: Suggests alternative activities when a primary choice is rejected due to constraints
- **generate_registration_plan**: Generates a comprehensive family activity itinerary including sequence, payments, and checklists
- **get_equipment_summary**: Compiles a consolidated list of all necessary items for a specific subset of activities
- **validate_activity_feasibility**: Checks if a specific activity can be added to an existing set of chosen activities without violating constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Activity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a registration plan for these activities: Swimming ($50, starts 2024-06-01, deadline 2024-05-25, gear: goggles), Hiking ($30, starts 2024-06-05, deadline 2024-05-30, gear: boots). My budget is $100, current date is 2024-05-20, and I need 1 hour between activities."

**🤖 AI Agent:**
> Your registration sequence is: 1. Swimming (Register by 2024-05-25), 2. Hiking (Register by 2024-05-30). Total cost is $80. Your equipment checklist includes: goggles, boots.

---

**👤 You:**
> "Check if a Museum trip ($40, starts 2024-07-10) is feasible with my current plan: Swimming ($50, starts 2024-06-01) and a budget of $80."

**🤖 AI Agent:**
> No, the Museum trip is not feasible because it would exceed your remaining budget.

---

**👤 You:**
> "What equipment do I need for Swimming and Hiking?"

**🤖 AI Agent:**
> You will need: goggles, boots.


## ❓ FAQ

**Q: How does the tool handle budget constraints?**
The engine ensures the sum of all registration fees does not exceed the specified family budget. If an activity is too expensive, it will be flagged in the conflicts section.

**Q: Can it manage travel time between activities?**
Yes, by using the `transportBuffer` parameter, the tool prevents scheduling overlaps by accounting for the time needed to travel between locations.

**Q: What happens if a registration deadline has passed?**
The tool checks the `currentDate` against all activity deadlines. If a deadline has passed, that activity will be excluded from the plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-activity-planner](https://vinkius.com/en/ai-agent-connect/family-activity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Activity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-activity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Activity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-activity-planner": {
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
