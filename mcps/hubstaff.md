# Hubstaff MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubstaff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze timesheets, query organizational lists, and manage team activities via Hubstaff seamlessly from any AI agent.

## Description
Connect your **Hubstaff** tracking account to any AI agent and bring your entire workforce analytics straight to a conversational interface.

### What you can do

- **Track Activities** — Investigate how time is allocated pulling detailed tracked activities and daily activity snapshots
- **Workforce Management** — Analyze organizations, users, and tasks without toggling native dashboard panels
- **Project Analytics** — Determine the list of created projects and fetch precise timesheets for agile billing summaries

### How it works

1. Subscribe to this server
2. Enter your Personal Access Token from Hubstaff V2
3. Start fetching and building project insights via Claude or Cursor immediately

### Who is this for?

- **HR Leadership** — pull daily timesheet overviews directly through text queries dynamically
- **Project Managers** — connect task structures easily without losing overview of sprint tabs
- **Freelancers** — automatically verify daily tracked times quickly at the command line


## Available Tools (9)
- **get_organization**: Get parameters surrounding an organization
- **get_project**: Retrieve single project structure
- **get_user**: Fetch targeted user details
- **list_activities**: Retrieve global organizational activities logged
- **list_organizations**: Retrieve the parent organizations
- **list_projects**: Retrieve all active projects linked to an organization
- **list_tasks**: Retrieve operational sub-tasks per project
- **list_time_entries**: Read explicitly billed or logged temporal time blocks
- **list_users**: Retrieve staff and employees under the hub


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hubstaff** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check my Hubstaff dashboard and list the organizations I have access to?"

**🤖 AI Agent:**
> Absolutely. I found 1 registered organization called 'Central Dev Agency' under the ID block 50293.

---

**👤 You:**
> "Retrieve all the timesheets available so I can verify billing."

**🤖 AI Agent:**
> Inspecting timesheets... The endpoint has returned 3 fresh entries logging roughly 18 active worked hours combined across your teams.

---

**👤 You:**
> "List today's daily activities tracked in the organization."

**🤖 AI Agent:**
> Checking daily logs... I've retrieved today's activity entries. User Sarah has 4 hours tracked with an 85% average activity score.


## ❓ FAQ

**Q: How do I get started?**
Subscribe, enter your API credentials (your generated Hubstaff PAT via **User Settings → Personal access tokens**), and you're set. No code, no environment files, no postbacks — just connect and audit team activity with natural text.

**Q: Can my AI check a single associate's daily activities quickly?**
Yes! Direct your prompt to fetch all logged daily activities (or activities specifically). The agent will query Hubstaff, breaking down the tracking records and formatting them directly so you won't need to manually click through web portals.

**Q: How easy is it to gather organization and project specifics?**
It essentially takes seconds explicitly asking 'List my organizations and projects.' The `list_projects` functionality traverses your environment returning the IDs you need to inspect underlying items.

**Q: Is the agent suited to handle multiple large organizational hubs at once?**
Yes! Due to targeted parameter queries (e.g., retrieving timesheets by target organization), HR firms and agencies scaling hundreds of contractors can extract clean textual aggregations pain-free via simple prompts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubstaff](https://vinkius.com/mcp/hubstaff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hubstaff** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubstaff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hubstaff** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubstaff": {
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
