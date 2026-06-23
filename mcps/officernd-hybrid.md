# OfficeRnD Hybrid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/officernd-hybrid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Hybrid work management — book desks, rooms, and manage office resources via OfficeRnD.

## Description
Connect your **OfficeRnD Hybrid** account to empower your AI agents with office management capabilities. This server allows for seamless scheduling and resource coordination.

### What you can do

- **Desk & Room Booking** — Instantly create or cancel bookings for desks and meeting rooms
- **Resource Discovery** — List all available office resources, locations, and floors
- **Team Coordination** — View organization teams and employee directories
- **Event Monitoring** — Keep track of upcoming office events and community activities

### How it works

1. Subscribe to this server
2. Enter your **Client ID**, **Client Secret**, and **Org Slug**
3. Start managing your hybrid workspace from Claude, Cursor, or any MCP client


## Available Tools (10)
- **cancel_booking**: Cancel an existing booking
- **create_booking**: Create a new booking
- **get_booking**: Get a specific booking
- **get_my_profile**: Get current user profile
- **list_bookings**: List all bookings
- **list_employees**: List all employees
- **list_events**: List organization events
- **list_locations**: List organization locations
- **list_resources**: List all resources (desks, rooms, etc.)
- **list_teams**: List organization teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OfficeRnD Hybrid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available desks for today."

**🤖 AI Agent:**
> Fetching resources... I've found 12 available desks in the Main Office. Would you like to book one?

---

**👤 You:**
> "Book meeting room 'Zenith' for 2 PM today."

**🤖 AI Agent:**
> Creating booking for 'Zenith'... Success! Your reservation is confirmed from 2:00 PM to 3:00 PM.

---

**👤 You:**
> "Show my upcoming bookings."

**🤖 AI Agent:**
> Retrieving your bookings... You have a desk reserved for tomorrow at 9:00 AM and a meeting at 4:00 PM.


## ❓ FAQ

**Q: Where do I find my API credentials?**
Log in to the OfficeRnD Admin Portal, go to Settings > Developer Tools, and create a new application to get your Client ID and Secret.

**Q: What is the Organization Slug?**
The slug is the unique identifier for your organization in OfficeRnD, found in Settings > My Account.

**Q: Can I book a resource for someone else?**
The current tools perform actions on behalf of the authenticated application/user. Advanced delegation depends on your API permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/officernd-hybrid](https://vinkius.com/mcp/officernd-hybrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OfficeRnD Hybrid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `officernd-hybrid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OfficeRnD Hybrid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "officernd-hybrid": {
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
