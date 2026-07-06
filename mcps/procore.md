# Procore MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/procore)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Manage construction projects via Procore — track RFIs, submittals, punch lists, daily logs, and drawings from any AI agent.

## Description
Connect your **Procore** construction management platform to any AI agent and oversee projects, quality, and field operations through natural conversation.

### What you can do

- **Projects Overview** — List all active construction projects with status, addresses, timelines, and budget summaries
- **RFIs & Submittals** — Track Requests for Information and material approvals with assignees, due dates, and response histories
- **Field Observations** — Review safety and quality observations from the jobsite including priority, photos, and corrective actions
- **Punch Lists** — Monitor deficiencies to resolve before closeout with locations, assignees, and deadlines
- **Daily Logs** — Access daily logs with weather, workforce counts, equipment usage, and delay notes
- **Drawings** — Browse blueprints, elevations, and shop drawings with revision tracking

### How it works

1. Subscribe to this server
2. Enter your Procore Client ID, Client Secret, and Company ID from developers.procore.com
3. Start managing your construction projects from Claude, Cursor, or any MCP-compatible client

Procore is the leading cloud-based construction management software, connecting project teams across the entire building lifecycle.

### Who is this for?

- **Project Managers** — get instant status updates on RFIs and submittals without logging into Procore between site visits
- **Superintendents** — review daily logs and punch items for multiple projects in a single conversation
- **Quality & Safety Managers** — pull observation reports and track corrective actions across the entire portfolio


## Available Tools (8)
- **list_observations**: Includes type, priority, assignee, photos, and status.

List field observations
- **list_punch_items**: Includes description, location, assignee, due date, and status.

List punch list items
- **list_daily_logs**: Includes weather, workforce count, equipment, notes, and delays.

List daily construction logs
- **list_drawings**: Includes discipline, set, revision, and approval status.

List project drawings
- **list_projects**: List all construction projects
- **get_project**: Includes budget, schedule, team, and project settings.

Get project details
- **list_rfis**: Includes subject, status, assignee, due date, and response history.

List RFIs for a project
- **list_submittals**: Includes title, spec section, status, and approver.

List submittals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Procore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my active construction projects."

**🤖 AI Agent:**
> You have 4 active projects:
1. Skyline Tower (ID: 2847) — Mixed-use, 42 floors — 67% complete
2. Harbor View Apartments (ID: 3102) — 120 units — 34% complete
3. Metro Station Expansion (ID: 2955) — Infrastructure — 81% complete
4. Civic Center Renovation (ID: 3280) — Pre-Construction
Which project would you like to dive into?

---

**👤 You:**
> "List all overdue RFIs on the Skyline Tower project."

**🤖 AI Agent:**
> 2 overdue RFIs on Skyline Tower:
1. RFI-142: "Steel connection detail at Level 28" — Smith Engineering — 5 days overdue
2. RFI-156: "MEP conflict — HVAC vs. sprinkler routing" — Torres MEP — 2 days overdue
Both blocking work on floors 27-30. Check pending submittals too?

---

**👤 You:**
> "How many open punch items on Harbor View?"

**🤖 AI Agent:**
> 23 open punch items on Harbor View (3102):
• Unit interiors: 14 (paint, fixtures, hardware)
• Common areas: 6 (lobby tile, elevator, parking)
• Exterior: 3 (landscaping, sidewalk, lighting)
8 items due before March 30 inspections. Show the full list?


## ❓ FAQ

**Q: Can my AI give me a full project status including open RFIs, pending submittals, and punch items?**
Yes! Ask 'Give me a full status for project 2847.' It calls `list_rfis`, `list_submittals`, and `list_punch_items` to compile a consolidated briefing: 4 open RFIs (2 overdue), 7 pending submittals, and 12 punch items. A field-ready summary in seconds.

**Q: How can I review what happened on my jobsite yesterday?**
Ask 'Show me yesterday's daily log for project 2847.' The `list_daily_logs` tool returns weather, workforce headcount by trade, equipment on site, work completed, delays, and superintendent notes. Your complete jobsite briefing without a single phone call.

**Q: Is this integration read-only?**
Yes, entirely read-only. All 8 tools list and retrieve data — none can create, modify, or delete project records. Your OAuth credentials control which projects are accessible, matching your Company Admin permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/procore](https://vinkius.com/mcp/procore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Procore** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `procore` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Procore** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "procore": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
