# Bevy Community MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bevy-community)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage your community events and chapters via Bevy — list events, attendees, and chapters directly from any AI agent.

## Description
Connect your **Bevy Community** account to any AI agent and orchestrate your virtual and in-person event workflows through natural conversation.

### What you can do

- **Event Oversight** — List and inspect all community events, including dates, locations, and descriptions.
- **Chapter Management** — Access and manage community chapters (groups) and their regional distribution.
- **Attendee Analysis** — Retrieve lists of attendees for specific events to monitor community growth.
- **Event Discovery** — Search for events and chapters using keywords to find relevant community activities.
- **Metric Tracking** — Get real-time counts of events by status (upcoming, completed, etc.) for reporting.
- **User Insights** — List which chapters a specific user belongs to for better community mapping.

### How it works

1. Subscribe to this server
2. Enter your Bevy Subdomain and API Token
3. Start managing your community from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — quickly check event schedules and attendee lists without manual dashboard exports.
- **Developer Relations Leads** — monitor chapter activity and regional growth straight from their workspace.
- **Event Organizers** — retrieve event counts and type summaries for periodic reporting.


## Available Tools (10)
- **get_chapter**: Get specific chapter details
- **get_event_counts**: Retrieve counts of events by status
- **get_event**: Get specific event details
- **list_chapters**: List all community chapters
- **list_event_attendees**: List attendees for a specific event
- **list_event_types**: List available event types/categories
- **list_events**: List all community events
- **list_user_chapters**: List chapters a specific user belongs to
- **search_chapters**: Search for chapters by keyword
- **search_events**: Search for events by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bevy Community** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming events in our community."

**🤖 AI Agent:**
> I've retrieved your upcoming events. You have 3 events scheduled: 'Dev Meetup London' (ID: ev_1), 'Spring Product Launch' (ID: ev_2), and 'Community Breakfast' (ID: ev_3).

---

**👤 You:**
> "Search for events matching 'SaaS'."

**🤖 AI Agent:**
> I found 2 events matching 'SaaS': 'SaaS Growth Workshop' (ID: ev_992) and 'Enterprise SaaS Summit' (ID: ev_995). Would you like to see the attendee list for either?

---

**👤 You:**
> "Show the count of completed events this month."

**🤖 AI Agent:**
> Retrieving event counts... This month, your community has successfully completed 12 events across 5 different chapters.


## ❓ FAQ

**Q: Can I see the list of attendees for a specific event?**
Yes! Use the `list_event_attendees` tool with the Event ID. Your agent will fetch the full list of community members registered for that event.

**Q: How do I find community chapters in a specific region?**
Simply ask the agent to `search_chapters` with the region name as a query. It will retrieve all matching community groups located in that area.

**Q: Does the integration allow me to update event details?**
Currently, the toolset focuses on querying and monitoring (Read-Only). You can list and inspect events, attendees, and chapters, but creation or modification must be done through the Bevy HQ dashboard for security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bevy-community](https://vinkius.com/mcp/bevy-community)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bevy Community** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bevy-community` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bevy Community** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bevy-community": {
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
