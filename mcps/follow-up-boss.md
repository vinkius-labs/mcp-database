# Follow Up Boss MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/follow-up-boss)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage real estate leads, track deals, and oversee follow-up tasks via AI agents with Follow Up Boss.

## Description
Connect your **Follow Up Boss** (FUB) account to any AI agent to automate your real estate lead management and sales pipelines through the Model Context Protocol (MCP). Follow Up Boss is the central hub for high-growth real estate teams to convert more leads into closings. This MCP server enables you to manage your contacts, track deals, and handle follow-up tasks directly through natural conversation.

### What you can do

- **Lead Management** — List all contacts, fetch detailed profile metadata, and create new leads or people instantly.
- **Deal Tracking** — Monitor sales opportunities and pipelines by listing and retrieving specific deal metadata.
- **Task Oversight** — Create and manage follow-up tasks and reminders to ensure no lead falls through the cracks.
- **Engagement Insights** — Retrieve notes attached to contacts and add new updates to lead timelines from your chat interface.
- **Smart Filters** — Access your 'Smart Lists' to quickly identify which leads require immediate attention.
- **Activity Tracking** — Monitor website activity events such as property views and registrations.
- **Team Coordination** — List all CRM users and agents to maintain full context of your team's assignments.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Follow Up Boss API Key (found in Admin > API)
3. Start managing your real estate leads from Claude, Cursor, or any MCP client

### Who is this for?

- **Real Estate Agents** — quickly pull contact details or add notes while on the go via simple AI commands.
- **Team Leaders** — get an overview of team assignments and deal progress across the entire pipeline.
- **Lead Coordinators** — automate the organization of new inquiries and follow-up tasks without switching apps.


## Available Tools (12)
- **add_note**: Add a note to a contact
- **create_person**: Create a new contact
- **create_task**: Add a new task
- **get_deal**: Get deal details
- **get_person**: Get contact details
- **list_deals**: List sales opportunities (deals)
- **list_events**: List website activity events
- **list_person_notes**: List notes for a contact
- **list_people**: List contacts (people)
- **list_smart_lists**: List smart filters (Smart Lists)
- **list_tasks**: List follow-up tasks
- **list_crm_users**: List team members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Follow Up Boss** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 people added to my CRM."

**🤖 AI Agent:**
> Retrieving contacts... I found 5 recent people, including 'John Smith' and 'Jane Doe'. Would you like the full profile for any of them?

---

**👤 You:**
> "Create a task for John Smith (ID: 123) to 'Follow up on contract' for tomorrow."

**🤖 AI Agent:**
> Task created! I've added a follow-up reminder for John Smith for tomorrow. You'll see it in your FUB dashboard.

---

**👤 You:**
> "Add a note to Jane Doe (ID: 456): 'Interested in waterfront properties'."

**🤖 AI Agent:**
> Note added! I've successfully posted the update to Jane Doe's timeline. Your team will see this interest recorded.


## ❓ FAQ

**Q: How do I get an API Key for Follow Up Boss?**
Admins can generate API keys in the Follow Up Boss dashboard under Admin > API.

**Q: Can I see notes for a specific contact?**
Yes, the 'list_person_notes' tool allows you to retrieve all notes associated with a specific person by their ID.

**Q: What are Smart Lists?**
Smart Lists are saved filters in Follow Up Boss that automatically group leads based on specific criteria (e.g., 'Leads to call today').

**Q: Can I update a lead's status via the agent?**
You can use the 'updateTask' or other modification tools to manage engagement. Status updates are pushed directly to the FUB core CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/follow-up-boss](https://vinkius.com/mcp/follow-up-boss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Follow Up Boss** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `follow-up-boss` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Follow Up Boss** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "follow-up-boss": {
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
