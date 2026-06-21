# Dryfta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dryfta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage event attendees, track sessions, and monitor abstract submissions via the Dryfta API.

## Description
Integrate **Dryfta**, the all-in-one event management platform, directly into your AI workflow. Manage your event attendees and registration statuses, track scheduled sessions and speaker assignments, monitor abstract submissions and review cycles, and oversee your event exhibitors using natural language.

### What you can do

- **Attendee Oversight** — List and retrieve detailed information and registration status for all your event participants.
- **Program Intelligence** — Monitor event sessions, workshops, speaker profiles, and real-time venue assignments.
- **Abstract Management** — Track submitted abstracts for your call for papers, including authors and current review statuses.
- **Exhibitor Monitoring** — List all event exhibitors and sponsors, resolving booth assignments and sponsorship levels.

### How it works

1. Connect the Dryfta integration to your AI assistant.
2. Authorize using your Dryfta subdomain and API Key.
3. Orchestrate your event planning and attendee management through intuitive conversation.

### Who is this for?

- **Event Managers** — Quickly check registration volumes and session schedules on the go.
- **Program Chairs** — Monitor abstract submission progress and review statuses via chat.
- **Operations Teams** — Research specific attendee details and exhibitor assignments instantly.


## Available Tools
- **get_dryfta_account_metadata**: Retrieve metadata and limits for your Dryfta account
- **get_attendee_details**: Get detailed profile and registration status for a specific attendee
- **quick_event_enrollment_audit**: Retrieve a high-level summary of attendee registration volumes
- **get_session_details**: Get detailed information and speaker list for a specific session
- **list_submitted_abstracts**: List all abstracts submitted for the event (call for papers)
- **list_event_attendees**: List all attendees registered for your Dryfta event
- **list_event_exhibitors**: List all exhibitors and sponsors registered for the event
- **list_event_sessions**: List all scheduled sessions and workshops in the event program
- **list_upcoming_sessions**: Identify sessions that are scheduled to start soon (mock logic)
- **search_attendees_by_keyword**: Search for attendees using a name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dryfta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all registered attendees for our conference."

**🤖 AI Agent:**
> I've found several registered attendees, including 'Alice Johnson' (Standard) and 'Bob Miller' (VIP). Would you like to see the contact details for any of these participants?

---

**👤 You:**
> "Show me the sessions scheduled for tomorrow."

**🤖 AI Agent:**
> Tomorrow's sessions include 'AI in Healthcare' at 10:00 AM (Room A) and 'Future of MCP' at 2:00 PM (Main Hall). Should I pull the speaker list for the AI session?

---

**👤 You:**
> "Check the status of submitted abstracts."

**🤖 AI Agent:**
> I've retrieved 12 submitted abstracts. 5 are 'Under Review', 3 are 'Accepted', and 4 are 'Pending'. Would you like a list of the accepted abstract titles?


## ❓ FAQ

**Q: How do I get a Dryfta API Key?**
Log in to your Dryfta event dashboard, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. You will also need your event subdomain.

**Q: Can the agent register new attendees?**
This integration currently focuses on listing and auditing event data. New registrations and payments should be managed through your Dryfta event website registration forms.

**Q: Does the integration show session speakers?**
Yes, you can use the get_session_details tool to retrieve detailed information for specific sessions, which includes identifying the associated speaker profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dryfta](https://vinkius.com/mcp/dryfta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dryfta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dryfta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dryfta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dryfta": {
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
