# Eventmaker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventmaker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage events, track participants, and monitor check-ins via the Eventmaker API.

## Description
Integrate **Eventmaker**, the comprehensive event management software, directly into your AI workflow. Manage your corporate events and trade shows, track registered participants and exhibitors, monitor session schedules and real-time check-ins, and oversee your event performance using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, start dates, and status for all your Eventmaker projects.
- **Participant Intelligence** — Monitor registered participants and exhibitors, resolving names, emails, and professional categories.
- **Operational Management** — Access and monitor event sessions and real-time check-in logs to stay ahead of attendee flow.
- **Performance Auditing** — Retrieve high-level summaries of registration volume, check-in rates, and organizational event health instantly.

### How it works

1. Connect the Eventmaker integration to your AI assistant.
2. Authorize using your Eventmaker API Key (found in your account settings).
3. Orchestrate your event planning and onsite operations through intuitive conversation.

### Who is this for?

- **Event Managers** — Quickly check participant counts and check-in logs on the go.
- **Marketing & Sales Teams** — Research exhibitor details and session popularity via chat during the event.
- **Operations Teams** — Monitor registration progress and organizational event metadata instantly.


## Available Tools
- **get_eventmaker_account_metadata**: Retrieve metadata and limits for your Eventmaker account
- **get_event_performance_stats**: Get high-level performance metrics for a specific event
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_engagement_audit**: Retrieve a high-level summary of participants and check-ins
- **list_currently_ongoing_events**: Identify events that are currently active or ongoing
- **list_event_checkins_log**: List all check-in events and logs for a specific event
- **list_all_events**: List all events managed in your Eventmaker account
- **list_event_exhibitors**: List all exhibitors and partners for a specific event
- **list_event_participants**: List all registered participants for a specific event
- **list_event_sessions**: List all sessions and schedule items for a specific event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventmaker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all participants for event ID '12345'."

**🤖 AI Agent:**
> I've found 150 participants for event '12345', including 'Alice Johnson' (Marketing Manager), 'Robert Smith' (Exhibitor), and 'David Williams'. Would you like the contact information for Alice Johnson?

---

**👤 You:**
> "Show me the check-in log for today."

**🤖 AI Agent:**
> I've retrieved the check-in log for today. 85 participants have checked in so far, with peak arrival between 9:00 AM and 10:00 AM. 5 exhibitors have also arrived. Would you like a list of participants currently checked in?

---

**👤 You:**
> "Get performance stats for 'Autumn Trade Show'."

**🤖 AI Agent:**
> The 'Autumn Trade Show' has 1,200 registrations and a 75% check-in rate. Session 'New Tech Demo' was the most attended. 45 leads were scanned by exhibitors on average. Should I check the detailed session breakdown?


## ❓ FAQ

**Q: How do I get an Eventmaker API Key?**
Log in to your Eventmaker account, navigate to **Account Settings > API**, and you can generate or retrieve your unique API Key from there. Ensure you have an active plan that supports API access.

**Q: Can the agent perform onsite check-ins?**
This integration currently focuses on listing and auditing events, participants, and check-in logs. Performing live check-ins or scanning badges should be managed via the Eventmaker mobile app or onsite hardware.

**Q: Does the integration show real-time attendance rates?**
Yes, you can use the get_event_performance_stats tool to retrieve real-time data on check-in rates and total registrations compared to onsite attendance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventmaker](https://vinkius.com/mcp/eventmaker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eventmaker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eventmaker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eventmaker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventmaker": {
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
