# Weekly Household Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-household-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate household chores, meals, and appointments into an optimized weekly schedule.

## Description
This MCP server acts as a coordination engine for managing household logistics. It reconciles member availability, recurring chores, fixed appointments, and meal slots against prioritized household rules. Use `generate_weekly_schedule` to produce a complete plan, `get_member_availability` to check if someone is free, `list_unassigned_tasks` to find leftover work, and `resolve_scheduling_conflict` to fix overlaps. It is designed to work with Cursor, VS Code, Claude Desktop, and Windsurf via Vinkius Edge.


## Available Tools (4)
- **generate_weekly_schedule**: Produces the complete organized plan for the week
- **get_member_availability**: Checks if a specific member is free to take on work at a given time
- **list_unassigned_tasks**: Identifies chores or meal slots that have not yet been allocated to a member
- **resolve_scheduling_conflict**: Suggests a different member or time slot to fix a specific overlap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Household Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate the weekly schedule for my household."

**🤖 AI Agent:**
> Here is your weekly schedule: Monday: John (Laundry), Sarah (Dishes). Tuesday: John (Grocery Shopping). No conflicts detected.

---

**👤 You:**
> "Are there any chores that haven't been assigned yet?"

**🤖 AI Agent:**
> Yes, the following tasks are unassigned: Vacuuming (High Priority) and Trash Collection (Low Priority).

---

**👤 You:**
> "Is Sarah available on Wednesday between 2 PM and 4 PM?"

**🤖 AI Agent:**
> Yes, Sarah is available during that time window.


## ❓ FAQ

**Q: How do I generate my weekly plan?**
You can use the `generate_weekly_schedule` tool to create a full breakdown of assignments, conflicts, and unassigned tasks.

**Q: What happens if there is a scheduling clash?**
You can use `resolve_scheduling_conflict` to find a better time slot or a different household member to handle the task.

**Q: Can I check if a specific person is free?**
Yes, use `get_member_availability` by providing the member ID and the time window you want to check.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-household-planner](https://vinkius.com/en/ai-agent-connect/weekly-household-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Household Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-household-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Household Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-household-planner": {
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
