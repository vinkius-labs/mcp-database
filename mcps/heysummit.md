# HeySummit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heysummit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Launch virtual summits and online conferences with speaker management, attendee registration, and engagement tracking built in.

## Description
Connect your **HeySummit** account to any AI agent and take full control of your online event management and summit workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and manage multiple online summits and retrieve detailed event metadata
- **Attendee Management** — Register new participants and track existing attendee lists to keep your audience engaged
- **Content Organization** — Manage event talks, categories, and speaker profiles programmatically to maintain a perfect schedule
- **Speaker Coordination** — Retrieve detailed speaker information and bios to automate professional event promotion
- **Real-time Monitoring** — Check registration status and event progress directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your API Key from the HeySummit Event Setup dashboard (API Settings)
3. Start managing your online summits from Claude, Cursor, or any MCP client

No more manual attendee tracking or schedule updates through complex web forms. Your AI acts as your dedicated event coordinator.

### Who is this for?

- **Event Organizers** — scale attendee management and speaker coordination for large-scale online summits
- **Marketing Teams** — automate lead registration and track event performance through natural language queries
- **Community Managers** — keep your members updated on event schedules and speaker lineups without leaving your workspace


## Available Tools
- **add_attendee**: Register a new attendee
- **get_event**: Get event details
- **get_me**: Get account information
- **get_speaker**: Get speaker details
- **get_talk**: Get talk details
- **list_attendees**: List event attendees
- **list_categories**: List event categories
- **list_events**: List all events
- **list_speakers**: List event speakers
- **list_talks**: List event talks
- **list_tickets**: List event tickets
- **update_event**: Update an existing event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HeySummit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active summits in my HeySummit account."

**🤖 AI Agent:**
> I've retrieved your events. You have 2 active summits: 'Global AI Expo 2026' (ID: 12345) and 'SaaS Leadership Summit' (ID: 67890). Which one would you like to drill into?

---

**👤 You:**
> "Show me the schedule of talks for event ID '12345'."

**🤖 AI Agent:**
> Fetching schedule for event 12345... I found 5 scheduled talks. Highlights include 'The Future of MCP' by Dr. Smith and 'Scaling AI Infrastructure'. Would you like the full speaker details for any of these?

---

**👤 You:**
> "Register 'john.doe@example.com' as an attendee for summit 12345."

**🤖 AI Agent:**
> Registration successful! John Doe (john.doe@example.com) is now registered for 'Global AI Expo 2026'. They will receive a confirmation email shortly.


## ❓ FAQ

**Q: Where do I find the Event ID for a specific summit?**
You can use the `list_events` tool to retrieve a list of all summits in your account. Each entry will include its unique numeric ID and name.

**Q: Can the agent handle speaker details and bios?**
Yes! The `list_speakers` tool allows your agent to fetch professional profiles, bios, and social links for all speakers associated with an event.

**Q: How do I register a new attendee programmatically?**
Use the `create_attendee` tool by providing the `event_id`, email, and name. The agent will confirm the registration status immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heysummit](https://vinkius.com/mcp/heysummit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HeySummit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `heysummit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HeySummit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heysummit": {
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
