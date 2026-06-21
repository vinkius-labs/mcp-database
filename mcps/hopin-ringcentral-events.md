# Hopin (RingCentral Events) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hopin-ringcentral-events)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Connect and manage RingCentral Events (formerly Hopin) webinars and virtual events.

## Description
Empower your AI agents to manage your virtual events ecosystem. This MCP server provides access to RingCentral Events (Hopin) API to list events, manage registrations, track schedules, speakers, and sessions. Ideal for automating event logistics and attendee management.


## Available Tools (10)
- **create_registration**: Registers a user for an event
- **get_event**: Retrieves details for a specific event
- **list_events**: Lists events in your RingCentral Events (Hopin) organization
- **list_organizations**: Lists organizations associated with your account
- **list_registrations**: Lists attendees/registrations for an event
- **list_schedule**: Lists the schedule items for an event
- **list_sessions**: Lists interactive sessions for an event
- **list_speakers**: Lists speakers for an event
- **list_tickets**: Lists tickets configured for an event
- **list_vendors**: Lists vendors/exhibitors for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hopin (RingCentral Events)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming events in my organization."

**🤖 AI Agent:**
> I'll fetch your organization's events.

---

**👤 You:**
> "Get the schedule for the event with ID 123."

**🤖 AI Agent:**
> I'll retrieve the schedule for that event.

---

**👤 You:**
> "Show me the list of speakers for event 456."

**🤖 AI Agent:**
> I'll fetch the speakers lineup for you.


## ❓ FAQ

**Q: Is this the same as Hopin?**
Yes, Hopin was acquired and rebranded as RingCentral Events. This MCP uses the official RingCentral Events API.

**Q: How do I get an Access Token?**
You can generate an Access Token in the RingCentral Events Developer Portal by creating an application.

**Q: Can I register attendees with this MCP?**
Yes, the create_registration tool allows you to register new attendees for any specific event.

**Q: Does it support organization management?**
The MCP allows you to list organizations to find your IDs and metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hopin-ringcentral-events](https://vinkius.com/mcp/hopin-ringcentral-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hopin (RingCentral Events)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hopin-ringcentral-events` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hopin (RingCentral Events)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hopin-ringcentral-events": {
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
