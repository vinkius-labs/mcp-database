# BoardEffect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boardeffect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage board activities via BoardEffect — list meetings, members, and documents directly from any AI agent.

## Description
Connect your **BoardEffect (Diligent)** account to any AI agent and orchestrate your board management and governance workflows through natural conversation.

### What you can do

- **Meeting Oversight** — List and retrieve detailed information for board meetings, including agendas and dates.
- **Member Directory** — Access your directory of board members and retrieve detailed profiles and contact info.
- **Workroom Coordination** — List all workrooms and access specific committee documents and archives.
- **Governance Monitoring** — Retrieve board surveys and polls to track feedback and decision-making.
- **Archive Access** — List and retrieve historical board records and archived projects.
- **Account Integration** — Verify user profiles and organization settings directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BoardEffect API Token and Subdomain
3. Start managing your board governance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Board Administrators** — quickly check meeting schedules and member details without navigating the full portal.
- **Corporate Secretaries** — monitor document archives and survey statuses straight from their workflow tools.
- **Executives** — retrieve board member information and meeting summaries using natural language.


## Available Tools (10)
- **get_account_info**: Get current user account information
- **get_meeting**: Get specific meeting details
- **get_member**: Get specific member details
- **list_archives**: List archived board records
- **list_documents**: List documents in a specific workroom
- **list_meetings**: List all board meetings
- **list_members**: List all board members
- **list_polls**: List board polls
- **list_surveys**: List board surveys
- **list_workrooms**: List all workrooms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoardEffect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming board meetings."

**🤖 AI Agent:**
> I've retrieved your meetings. You have 3 upcoming sessions: 'Quarterly Strategy Review' (ID: meet_1), 'Audit Committee' (ID: meet_2), and 'Annual General Meeting' (ID: meet_3).

---

**👤 You:**
> "Show the documents in the 'Finance Committee' workroom."

**🤖 AI Agent:**
> Retrieving documents... I found 5 files, including 'Budget Draft Q3.pdf', 'Expense Report - Feb.pdf', and 'Investment Strategy.docx'. Would you like the details for any of these?

---

**👤 You:**
> "Find contact details for board member Sarah Miller."

**🤖 AI Agent:**
> I found one matching member: 'Sarah Miller' (ID: mem_992). Her email is sarah.miller@example.com and she is the Chair of the Audit Committee.


## ❓ FAQ

**Q: Can I see the agenda for my next board meeting?**
Yes! Use the `get_meeting` tool with the Meeting ID. Your agent will fetch the latest details, including the agenda and scheduled time, directly from BoardEffect.

**Q: How do I list all the members of a specific committee?**
Simply ask the agent to `list_members`. You can then inspect individual member profiles or use the `list_workrooms` tool to see which members are assigned to specific committee spaces.

**Q: Does the integration allow me to archive a project?**
Currently, the toolset focuses on querying and monitoring (Read-Only). You can list and inspect meetings, members, and archives, but archiving active projects or deleting data must be done through the BoardEffect platform for security and compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boardeffect](https://vinkius.com/mcp/boardeffect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoardEffect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boardeffect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoardEffect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boardeffect": {
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
