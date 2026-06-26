# Accelevents MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accelevents)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

All-in-one event management platform — manage events, attendees, and session registration via AI.

## Description
Connect your **Accelevents** account to your AI agent to unlock effortless event orchestration. From managing large-scale attendee lists to tracking real-time session registration, your agent handles event logistics through natural conversation.

### What you can do

- **Event Management** — List all your active, past, or upcoming events and retrieve technical metadata for each
- **Attendee Tracking** — List participants, search for specific profiles, and monitor ticket sales for your events
- **Session Registration** — Manage event sessions and track user registrations to ensure optimal capacity planning
- **Check-in Workflow** — Quickly audit attendee check-ins and identify engagement patterns during live events
- **Exhibitor Monitoring** — Retrieve details on exhibitors and products to support your event's marketplace


## Available Tools (4)
- **list_events**: Retrieve a list of all active, past, and upcoming events in Accelevents
- **list_exhibitors**: Requires the event URL.

Retrieve details on companies exhibiting at a specific Accelevents event
- **list_sessions**: Requires the event URL.

Retrieve the schedule and session details for an Accelevents event
- **list_attendees**: Requires the event URL.

Retrieve the participant list and ticket types for a specific Accelevents event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelevents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all upcoming events in my Accelevents account."

**🤖 AI Agent:**
> I've retrieved your upcoming events. You have 3 events scheduled for next month, including 'Tech Conference 2026'. Would you like to see the attendee count for any of them?


## ❓ FAQ

**Q: How do I list all attendees for a specific event?**
Use the `list_attendees` tool and provide the event URL (identifier). Your agent will retrieve the full list of participants, including their ticket types.

**Q: Are there extra limits for custom integrations?**
No, Accelevents provides public REST APIs and webhooks with no additional access fees for building your custom event workflows.

**Q: Can I receive real-time updates on ticket sales?**
Yes, you can configure webhooks to receive real-time notifications for specific topics, including ticket purchases and attendee check-ins.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accelevents](https://vinkius.com/mcp/accelevents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelevents** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelevents` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelevents** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelevents": {
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
