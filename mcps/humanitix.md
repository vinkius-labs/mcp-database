# Humanitix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/humanitix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage events, tickets, and attendees via Humanitix API.

## Description
Connect your AI agents to Humanitix, the humane ticketing platform. This MCP server allows you to list events, track ticket sales, manage attendee lists, and view organization data directly through the Humanitix API. Ideal for automating event logistics and community management while supporting social impact.


## Available Tools (10)
- **get_event**: Retrieves details for a specific event
- **get_me**: Gets current authenticated user info
- **list_attendees**: Lists attendees for a specific event
- **list_campaigns**: Lists marketing campaigns
- **list_events**: Lists virtual and hybrid events
- **list_hosts**: Lists event hosts
- **list_inventory**: Lists event inventory
- **list_orders**: Lists ticket orders
- **list_tickets**: Lists tickets across all events
- **list_venues**: Lists event venues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Humanitix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming charity events in my Humanitix account."

**🤖 AI Agent:**
> I'll fetch the list of upcoming events for you.

---

**👤 You:**
> "Show me the attendee list for the Annual Gala."

**🤖 AI Agent:**
> I'll retrieve the registered attendees for that event.

---

**👤 You:**
> "Check how many tickets are left for event ID 789."

**🤖 AI Agent:**
> I'll check the inventory and ticket availability for you.


## ❓ FAQ

**Q: How do I get Humanitix API credentials?**
You can find your API key in your Humanitix dashboard under Account Settings > API. Ensure you have the necessary permissions to access event data.

**Q: Can I see attendee emails?**
Yes, the list_attendees tool provides access to registered attendee details including contact information if available.

**Q: Is inventory management supported?**
Yes, the list_inventory tool allows you to track ticket availability and stock levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/humanitix](https://vinkius.com/mcp/humanitix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Humanitix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `humanitix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Humanitix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "humanitix": {
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
