# Luma MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/luma)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Host and manage events beautifully with registration pages, attendee communication, and analytics for in-person and virtual gatherings.

## Description
Connect your **Luma** (lu.ma) account to any AI agent and take full control of your event orchestration and community engagement through natural conversation. Luma provides a robust platform for managing calendars and events, and this integration allows you to retrieve event metadata, manage guest lists, and create new activities directly from your chat interface.

### What you can do

- **Event & Calendar Orchestration** — List all managed events and retrieve detailed metadata programmatically to ensure your community roadmap is always synchronized.
- **Guest Lifecycle Management** — Access and monitor guest lists and add new attendees directly from the AI interface to maintain high-fidelity event engagement.
- **Communication & Update Control** — List hosts and organizers linked to a calendar via natural language to drive better team alignment.
- **Organization Oversight** — Access organizational events and monitor system webhooks using simple AI commands.
- **Operational Monitoring** — Track system responses and manage event metadata to ensure your community workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Luma API Key (requires Luma Plus) from your calendar settings
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

No more manual logging into the dashboard for quick guest checks. Your AI acts as a dedicated event coordinator or community assistant.

### Who is this for?

- **Event Planners & Hosts** — quickly retrieve guest summaries and monitor event health without switching apps.
- **Community Managers** — automate the retrieval of attendee metadata and track community growth via natural conversation.
- **Growth Teams** — streamline the ingestion of new guests and monitor organizational activity directly within the chat.


## Available Tools (6)
- **add_guests_to_event**: Manually add guests to an event
- **create_event**: Create a new Luma event
- **list_event_guests**: List guests for an event
- **list_events**: List your Luma events
- **list_organization_events**: List all events in your organization
- **list_calendar_subscribers**: List subscribers to your calendar


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Luma** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Luma."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming activities including 'AI Workshop' and 'Community Meetup'. Which one would you like to see guest counts for?

---

**👤 You:**
> "Show me the guest list for the 'Product Launch' event."

**🤖 AI Agent:**
> I've retrieved the guest list. There are 45 confirmed attendees, including 10 VIPs. Would you like me to highlight any specific group?

---

**👤 You:**
> "Add 'sarah@example.com' to the workshop guest list."

**🤖 AI Agent:**
> Sarah has been successfully added to the 'AI Workshop' guest list. Would you like me to send her the calendar invitation now?


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific event by its ID?**
Yes! While the `list_events` tool retrieves all entries, you can use the event metadata to filter and focus on specific records. Your agent will respond with complete metadata for the record in seconds.

**Q: How do I find my Luma API Key?**
Log in to your Luma account, select your calendar, navigate to **Settings** > **Developer**, and you will find your unique secret token there. Note: You must have Luma Plus.

**Q: Can I add guests to an event via the AI?**
Absolutely. Use the `add_guests` tool. Provide the event ID and an array of guest objects (email and name), and the agent will register them to your event immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/luma](https://vinkius.com/mcp/luma)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Luma** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `luma` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Luma** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "luma": {
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
