# Airmeet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airmeet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Event management and orchestration — manage virtual events, attendees, and recordings via AI.

## Description
Connect your **Airmeet** community to your AI agent to unlock professional event orchestration and attendee management. From creating new virtual events and sessions to auditing attendee lists and retrieving session recordings, your agent handles your event lifecycle through natural conversation.

### What you can do

- **Event Orchestration** — Create and configure Airmeet events, manage sessions, and update event statuses (start, pause, end)
- **Attendee Management** — Add authorized attendees, retrieve magic links, and audit participant lists for any event
- **Speaker Coordination** — Add and manage speakers for your event sessions seamlessly
- **Engagement Auditing** — Retrieve analytics for event attendance, poll responses, and questions asked by participants
- **Media Access** — Retrieve download links for session recordings to support your post-event content strategy

### How it works

1. Subscribe to this server
2. Enter your Airmeet Access Key and Secret Key
3. Start managing your virtual events and monitoring engagement through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — automate attendee registration and monitor real-time event status effortlessly
- **Marketing Teams** — audit poll responses and participant engagement data for lead qualification
- **Community Managers** — quickly look up participant details and provide magic links via chat
- **Content Producers** — retrieve session recordings and audit speaker assignments using simple commands


## Available Tools
- **list_events**: List virtual events
- **create_event**: Create a new Airmeet
- **update_event_status**: Change event status
- **add_attendee**: Register an attendee
- **list_participants**: List event participants
- **create_session**: Add a session to event
- **get_event_attendance**: Get attendance analytics
- **list_poll_responses**: List event polls
- **list_questions**: List participant questions
- **get_session_recordings**: Get recording download links


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airmeet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Airmeet events scheduled for next month."

**🤖 AI Agent:**
> I've retrieved your upcoming events. You have 3 events scheduled for next month: 'Global Tech Summit', 'Customer Success Webinar', and 'Product Launch 2026'. Would you like to see the session details for any of them?

---

**👤 You:**
> "Add 'John Doe' (john@example.com) as an attendee to event ID 12345."

**🤖 AI Agent:**
> I've successfully added John Doe to the event. A magic link has been generated and he should receive an invitation email shortly. Would you like me to retrieve his unique entry URL for you now?

---

**👤 You:**
> "Retrieve the recordings for session ID 98765."

**🤖 AI Agent:**
> I've found 2 recording files for session 98765. I've prepared the download links for you; they will remain active for the next 6 hours. Would you like the links for both the video and audio-only versions?


## ❓ FAQ

**Q: How do I find my Airmeet Access and Secret Keys?**
Log in to your Airmeet Dashboard, navigate to **Integrations** > **API Access Key**, and click on 'Generate Key'. You will receive both the Access Key and Secret Key there.

**Q: Can I retrieve magic links for attendees?**
Yes! When you use the `add_attendee` tool, Airmeet generates a unique entry link. You can also use the `list_participants` tool to retrieve existing magic links for registered users.

**Q: How long are recording links valid?**
Recording download links retrieved via the `get_session_recordings` tool are temporary and typically remain valid for 6 hours. We recommend downloading the media immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airmeet](https://vinkius.com/mcp/airmeet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airmeet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `airmeet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airmeet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airmeet": {
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
