# EventMobi Experience MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventmobi-experience)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Equip your AI agent to manage event apps, track attendee engagement, and monitor sessions via the EventMobi API.

## Description
Integrate **EventMobi**, the comprehensive event experience platform, directly into your AI workflow. Manage your mobile event apps and schedules, track registered attendees and speaker profiles, monitor real-time engagement analytics and exhibitor visibility, and oversee your event success using natural language.

### What you can do

- **App Oversight** — List and retrieve detailed information, dates, and status for all your EventMobi event applications.
- **Attendee & Speaker Intelligence** — Monitor participant profiles and speaker bios, resolving professional roles and unique identifiers.
- **Engagement Management** — Access and monitor real-time app analytics, identifying session favorites and interaction rates.
- **Event Auditing** — Retrieve high-level summaries of attendee volume, session activity, and organizational event health instantly.

### How it works

1. Connect the EventMobi integration to your AI assistant.
2. Authorize using your EventMobi API Key (found in your account settings).
3. Orchestrate your event experience and app strategy through intuitive conversation.

### Who is this for?

- **Event Managers** — Quickly check attendee registration counts and session popularity on the go.
- **Marketing Teams** — Research exhibitor visibility and app engagement via chat during live events.
- **Operations Teams** — Monitor app updates and organizational event metadata instantly.


## Available Tools
- **get_eventmobi_account_metadata**: Retrieve metadata and limits for your EventMobi account
- **get_event_engagement_analytics**: Get high-level engagement analytics for a specific event
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_volume_audit**: Retrieve a high-level summary of attendees, sessions, and speakers
- **list_event_attendees**: List all registered attendees for a specific event
- **list_event_exhibitor_profiles**: List all exhibitor and company profiles for a specific event
- **list_all_events**: List all events managed in your EventMobi account
- **list_latest_event_projects**: Identify the most recently created or updated event projects
- **list_event_sessions**: List all sessions and schedule items for a specific event
- **list_event_speakers**: List all speakers registered for a specific event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EventMobi Experience** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active event apps."

**🤖 AI Agent:**
> I've found 3 active event apps, including 'Annual Leadership Retreat' and 'Sales Kickoff 2024'. The Leadership Retreat currently has 250 registered attendees. Would you like to see the session schedule for this event?

---

**👤 You:**
> "Show me engagement analytics for event ID '12345'."

**🤖 AI Agent:**
> For event ID '12345', I've retrieved the engagement report: 1,500 total app views, 450 session favorites, and 85 networking messages sent. Engagement is up 12% compared to the previous period. Should I check which session is most popular?

---

**👤 You:**
> "Search for attendees with the role 'Director'."

**🤖 AI Agent:**
> I've found 12 attendees with the 'Director' role, including 'Sarah Connor' (IT Director) and 'John Doe' (Marketing Director). All are registered for the main event. Would you like to see Sarah's full speaker bio?


## ❓ FAQ

**Q: How do I get an EventMobi API Key?**
Log in to your EventMobi account, navigate to **Settings > API Integration**, and you can generate or retrieve your unique API Key from there. API access is typically enabled for most enterprise plans.

**Q: Does the integration show real-time analytics?**
Yes, you can use the get_event_engagement_analytics tool to retrieve high-level engagement data such as app views and session interactions as reported by the EventMobi platform.

**Q: Can the agent send push notifications?**
This integration currently focuses on listing and auditing event data and analytics. Sending live push notifications or updating app content should be managed via the EventMobi Experience Manager dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventmobi-experience](https://vinkius.com/mcp/eventmobi-experience)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EventMobi Experience** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eventmobi-experience` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EventMobi Experience** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventmobi-experience": {
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
