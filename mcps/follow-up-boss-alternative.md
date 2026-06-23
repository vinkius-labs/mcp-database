# Follow Up Boss MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/follow-up-boss-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Convert real estate leads into closings with a CRM that routes inquiries, automates follow-ups, and tracks agent performance.

## Description
Connect your **Follow Up Boss** account to any AI agent and take full control of your real estate lead management and follow-up workflows through natural conversation.

### What you can do

- **Lead Orchestration** — List and manage your complete database of people and leads, including retrieving detailed contact profiles and communication history
- **Activity Monitoring** — Track real-time events such as website registrations, property inquiries, and inquiries from integrated portals like Zillow or Realtor.com
- **Team Collaboration** — Programmatically add internal team notes to lead profiles and manage follow-up tasks to ensure no opportunity falls through the cracks
- **Deal & Appointment Oversight** — Monitor real estate transactions, commissions, and upcoming property showings directly through your agent
- **System Automation** — List and manage configured webhooks and account settings to maintain high-fidelity synchronization with your other tools

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Follow Up Boss admin settings (Admin > API)
3. Start managing your real estate business from Claude, Cursor, or any MCP client

No more manual status checking or digging through CRM lists on the go. Your AI acts as your dedicated real estate operations assistant.

### Who is this for?

- **Real Estate Agents** — instantly retrieve lead details and log field activity using natural language commands
- **Team Leaders** — monitor team-wide lead engagement and pipeline health without opening the web dashboard
- **Inside Sales Agents (ISAs)** — automate lead triaging and task management through simple AI queries


## Available Tools (12)
- **log_lead_activity**: Log a new activity event
- **add_internal_note**: Add a note to a lead profile
- **create_new_lead**: Requires essential details like email or name.

Add a new lead to the CRM
- **create_followup_task**: Create a new task
- **get_lead_details**: Get details for a specific lead
- **list_calendar_appointments**: List showings and appointments
- **list_real_estate_deals**: List transactions and deals
- **list_recent_events**: List website and activity events
- **list_person_notes**: List notes for a specific person
- **list_leads**: List lead profiles (people)
- **list_followup_tasks**: List CRM tasks
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Follow Up Boss** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my new leads from the last 24 hours."

**🤖 AI Agent:**
> Scanning your CRM... I've found 3 new leads from the last 24 hours: 'John Doe' (from Zillow), 'Sarah Smith' (Direct), and 'Acme Corp'. Would you like the full profile for any of them?

---

**👤 You:**
> "Add an internal note to lead 'p_123': 'Interested in 3-bedroom houses in North London'."

**🤖 AI Agent:**
> Note added! I've successfully posted your comment to lead p_123's activity feed. Your team will see this update in the Follow Up Boss dashboard immediately.

---

**👤 You:**
> "Show me my upcoming property showings for today."

**🤖 AI Agent:**
> Checking your calendar... You have 2 showings today: '123 Maple St' at 2 PM with Jane Doe, and '456 Oak Ave' at 4:30 PM. I can provide the lead details for either session if needed.


## ❓ FAQ

**Q: How do I find my API Key in Follow Up Boss?**
Log in as an Admin, navigate to **Admin** > **API**, and click **Create API Key** to generate your unique token.

**Q: Can I filter leads by their recent activity?**
Yes! Use the `list_recent_events` tool to see who has registered or inquired lately across all your integrated channels.

**Q: How do I get a specific person's ID?**
Use the `list_leads` tool to retrieve your contact list. Each result includes a unique `id` which you can use for granular details or notes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/follow-up-boss-alternative](https://vinkius.com/mcp/follow-up-boss-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `follow-up-boss-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Follow Up Boss** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "follow-up-boss-alternative": {
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
