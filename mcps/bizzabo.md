# Bizzabo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bizzabo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate your event experience via Bizzabo — manage events, registrations, and attendees directly from any AI agent.

## Description
Connect your **Bizzabo** account to any AI agent and orchestrate your events, registrations, and attendee workflows through natural conversation.

### What you can do

- **Event Oversight** — List and retrieve detailed information for all your upcoming and past events.
- **Registration Tracking** — Query and monitor event registrations to track ticket sales and attendee growth.
- **Contact Management** — Access your directory of attendees, speakers, and exhibitors across all events.
- **Session & Speaker Coordination** — Retrieve schedules and speaker details to ensure your event runs smoothly.
- **Ticket Type Discovery** — List available registration types and form properties for specific events.

### How it works

1. Subscribe to this server
2. Enter your Bizzabo API Key
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — quickly check registration counts and event details without opening the dashboard.
- **Marketing Teams** — retrieve attendee lists and metadata straight from their workflow tools.
- **Ops Teams** — monitor session schedules and speaker details using natural language.


## Available Tools (10)
- **get_contact**: Get specific contact details
- **get_event**: Get specific event details
- **get_registration**: Get specific registration details
- **get_session**: Get details of a specific session
- **list_contacts**: List all contacts across events
- **list_events**: List all Bizzabo events
- **list_registration_types**: List ticket types for an event
- **list_registrations**: List registrants for a specific event
- **list_sessions**: List sessions for an event
- **list_speakers**: List speakers for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bizzabo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Bizzabo."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming events: 'Annual Conference 2024' (ID: ev_1), 'Tech Summit' (ID: ev_2), and 'Developer Meetup' (ID: ev_3).

---

**👤 You:**
> "Show the sessions for event ev_1."

**🤖 AI Agent:**
> Retrieving sessions... I found 5 sessions, including 'Keynote: Future of Events', 'Panel: Digital Transformation', and 'Workshop: Networking Skills'. Which one would you like more details on?

---

**👤 You:**
> "Find the registration details for ID reg_992."

**🤖 AI Agent:**
> Registration reg_992 belongs to John Doe (john@example.com). They registered for the 'Early Bird' ticket type on March 15th and the status is 'Approved'.


## ❓ FAQ

**Q: Can I check the registration count for a specific event?**
Yes! Use the `list_registrations` tool with the Event ID. Your agent will fetch the list of registrants, allowing you to see the total volume directly.

**Q: How do I see the schedule for my upcoming event?**
Simply ask the agent to `list_sessions` and provide the Event ID. It will retrieve all scheduled sessions, showing titles and timings.

**Q: Does the integration allow creating new events?**
Currently, the toolset is focused on querying and monitoring (Read-Only). You can list and inspect events, registrations, and contacts, but creating new events must be done through the Bizzabo platform directly for full configuration control.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bizzabo](https://vinkius.com/mcp/bizzabo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bizzabo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bizzabo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bizzabo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bizzabo": {
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
