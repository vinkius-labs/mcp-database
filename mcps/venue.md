# Venue MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/venue)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage event venues with booking calendars, client contracts, and catering coordination for wedding and conference spaces.

## Description
Connect your **Venue.live** account to any AI agent and simplify how you coordinate high-engagement virtual events, webinars, and interactive sessions through natural conversation.

### What you can do

- **Event Management** — List all upcoming webinars, create new events, and retrieve detailed configuration metadata.
- **Session Coordination** — List and manage individual sessions or breakout rooms associated with your events.
- **Speaker Registry** — Create and list guest speaker profiles to manage your event directory.
- **Attendee Tracking** — List registered participants for specific events to monitor growth and sign-ups.
- **Engagement Analytics** — Retrieve performance metrics and attendance data for completed events to measure success.
- **Recording Library** — List and access video recordings from past events for content repurposing.

### How it works

1. Subscribe to this server
2. Enter your Venue API Key (found in your workspace settings)
3. Start managing your virtual venue from Claude, Cursor, or any MCP client

### Who is this for?

- **Event Planners** — quickly retrieve speaker lists and session details via simple AI commands.
- **Marketing Managers** — monitor registration counts and check event analytics without leaving the workspace.
- **Community Leads** — automate the creation of new events and manage attendee lists directly via the AI assistant.


## Available Tools (10)
- **list_events**: live.

List virtual events and webinars
- **list_recordings**: List event recordings
- **list_event_registrations**: List event attendees
- **list_event_sessions**: List sessions for a specific event
- **list_speakers**: List guest speakers
- **create_event**: Create a new virtual event
- **create_speaker**: Register a new speaker
- **get_event_analytics**: Get event engagement analytics
- **get_event_details**: Get details of a specific event
- **get_me**: Get account information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venue** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming events in my Venue account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming sessions: 'Product Launch Keynote', 'User Feedback Webinar', and 'Q4 Strategy Review'. Which one would you like details on?

---

**👤 You:**
> "Show me the analytics for the 'Summer Webinar' (ID: ev_10293)."

**🤖 AI Agent:**
> Fetching analytics... The 'Summer Webinar' had 150 unique attendees with an average engagement time of 45 minutes. There were 25 questions asked in the chat. Shall I retrieve the attendee list?

---

**👤 You:**
> "Create a new event titled 'AI Workshop' for Dec 10th at 2 PM UTC."

**🤖 AI Agent:**
> Success! The 'AI Workshop' has been scheduled for 2024-12-10 at 14:00 UTC (ID: ev_8823). I've added the title and start time. Would you like to add a description or register a speaker now?


## ❓ FAQ

**Q: Can I list all the speakers registered in my Venue account?**
Yes! Use the `list_speakers` tool. Your agent will retrieve the complete directory of guest speakers registered in your workspace.

**Q: How do I see how many people registered for a specific event?**
Run the `list_event_registrations` query with your Event ID. The agent will return the list of all registered participants for that specific session.

**Q: Is it possible to retrieve engagement metrics for a past event?**
Absolutely. Use the `get_event_analytics` tool and provide the Event ID. The agent will return attendance and engagement data to help you measure success.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/venue](https://vinkius.com/mcp/venue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venue** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venue` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venue** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venue": {
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
