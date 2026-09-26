# Relative Care Visit Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/relative-care-visit-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured operational briefings for caregivers by organizing routines, access, and tasks.

## Description
This MCP server provides tools to prepare comprehensive care visit briefs. It organizes care activities into three distinct phases: Arrival, Visit, and Departure. Using `generate_visit_brief`, caregivers can consolidate visit dates, person routines, communication preferences, household access, and specific tasks into a single, chronological operational guide. It also includes tools like `get_routine_by_date` to retrieve daily schedules, `get_access_protocols` for entry and security instructions, and `validate_task_feasibility` to ensure all duties fit within the allocated time window.


## Available Tools (4)
- **get_routine_by_date**: Retrieves the specific daily routine applicable to a given calendar date
- **generate_visit_brief**: Creates a complete, chronologically organized brief for a single care visit
- **get_access_protocols**: Retrieves the entry and security instructions for a specific household
- **validate_task_feasibility**: Checks if the requested tasks can be realistically completed within the standard care window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Care Visit Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Prepare a care visit brief for July 15th, 2024. Routines: ['Morning walk at 9am', 'Breakfast at 10am']. Communication: 'Speak softly and maintain eye contact'. Access: 'Key is under the blue mat'. Contacts: '[{"name": "Jane Doe", "relation": "Daughter"}]'. Tasks: ['Unlock door', 'Assist with breakfast', 'Lock door']."

**🤖 AI Agent:**
> Arrival: Unlock door. Visit: Assist with breakfast. Departure: Lock door.

---

**👤 You:**
> "Check if these tasks are feasible for a 30-minute visit: ['Check vitals', 'Clean kitchen', 'Prepare meal']."

**🤖 AI Agent:**
> No, the estimated duration exceeds the 30-minute window.

---

**👤 You:**
> "What is the routine for 2024-05-20?"

**🤖 AI Agent:**
> The routine for May 20th includes: Morning walk at 9am and Breakfast at 10am.


## ❓ FAQ

**Q: How does the brief organize tasks?**
The `generate_visit_brief` tool automatically sorts tasks into Arrival, Visit, and Departure phases based on their nature.

**Q: Can I check if my tasks are too many for the visit time?**
Yes, you can use the `validate_task_feasibility` tool to compare your task list against the allocated time window.

**Q: How do I find the entry instructions for a home?**
You can use the `get_access_protocols` tool by providing the specific household identifier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/relative-care-visit-brief](https://vinkius.com/en/ai-agent-connect/relative-care-visit-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Care Visit Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-care-visit-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Care Visit Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-care-visit-brief": {
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
