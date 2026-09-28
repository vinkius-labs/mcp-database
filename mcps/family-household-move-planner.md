# Family Household Move Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-household-move-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate complex family moves with synchronized timelines for packing, school continuity, and child stability.

## Description
This MCP server acts as a specialized orchestration engine for family relocations. It manages the logistical and psychological complexities of moving a household by prioritizing school-continuity and child-access. Use `get_move_calendar` to build a master timeline, `get_packing_plan` to distribute workloads among helpers, `get_child_transition_plan` to ensure emotional stability for dependents, and `get_first_week_setup` to prioritize essential home infrastructure upon arrival.


## Available Tools (4)
- **get_child_transition_plan**: Identifies specific tasks required to maintain emotional and physical stability for children during the move
- **get_first_week_setup**: Creates an immediate action plan for the first seven days in the new residence
- **get_move_calendar**: Generates a chronological timeline of all major milestones and deadlines
- **get_packing_plan**: Determines who should pack what and when, based on available helpers and belongings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Household Move Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a move calendar for July 15th, 2025, considering school starts on August 1st and address updates due by June 30th."

**🤖 AI Agent:**
> Your move calendar is ready. Key milestones include: June 30th (Address Updates), July 15th (Move Day), and August 1st (School Start).

---

**👤 You:**
> "Help me plan the first week in our new 3-bedroom house after we move on October 10th."

**🤖 AI Agent:**
> Your first-week setup plan is ready. We will prioritize utilities and safety, followed by setting up sleeping quarters in the 3 rooms.

---

**👤 You:**
> "Who should pack the kitchen items and heavy furniture if I have two helpers available starting next week?"

**🤖 AI Agent:**
> Based on your helpers' availability, the kitchen items are assigned to Helper A for completion by next Friday, and heavy furniture is assigned to Helper B.


## ❓ FAQ

**Q: How does the tool handle school schedules?**
The `get_move_calendar` tool integrates school obligations into the master timeline to ensure moving tasks do not conflict with critical educational milestones.

**Q: Can I assign specific packing tasks to different people?**
Yes, `get_packing_plan` allows you to input a list of helpers and their availability to generate specific packing assignments.

**Q: How is child stability managed during the move?**
The `get_child_transition_plan` tool applies Child-Access Priority, ensuring high-priority comfort items are handled with care to maintain emotional stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-household-move-planner](https://vinkius.com/en/ai-agent-connect/family-household-move-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Household Move Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-household-move-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Household Move Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-household-move-planner": {
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
