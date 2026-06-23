# Hubilo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubilo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage virtual and hybrid events via Hubilo API.

## Description
Empower your AI agents to manage your virtual event strategy with Hubilo. This MCP server provides access to the Hubilo API to list events, manage attendees, track orders, view agenda sessions, and analyze booth performance. Perfect for event organizers and marketing teams.


## Available Tools (10)
- **get_booth_analytics**: Retrieves analytics data for exhibitor booths
- **get_event_details**: Retrieves details for a specific event
- **get_organizer_profile**: Gets details about the event organizer
- **list_attendees**: Lists attendees registered for an event
- **list_booth_categories**: Lists exhibitor booth categories for an event
- **list_events**: Lists virtual and hybrid events
- **list_orders**: Lists ticket orders for an event
- **list_sessions**: Lists agenda sessions for an event
- **list_speakers**: Lists speakers for an event
- **list_tickets**: Lists tickets for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hubilo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Hubilo."

**🤖 AI Agent:**
> I'll fetch your event list for you.

---

**👤 You:**
> "Show me the list of attendees for event ID 456."

**🤖 AI Agent:**
> I'll retrieve the attendee list for that event.

---

**👤 You:**
> "Check the agenda sessions for my virtual summit."

**🤖 AI Agent:**
> I'll look up the session list for your event.


## ❓ FAQ

**Q: How do I get a Hubilo Access Token?**
You can generate an Access Token in your Hubilo Dashboard under Integration Settings. You may need to contact your account manager if the option is not visible.

**Q: Can I see attendee lists?**
Yes, the list_attendees tool provides the full list of registered users for a specific event.

**Q: Is booth analytics supported?**
Yes, you can retrieve booth performance and analytics using the get_booth_analytics tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubilo](https://vinkius.com/mcp/hubilo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hubilo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubilo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hubilo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubilo": {
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
