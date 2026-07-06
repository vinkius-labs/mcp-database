# HQBeds MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hqbeds)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage hostel and accommodation bookings with channel distribution, guest communication, and occupancy tracking in one system.

## Description
Connect your **HQBeds** account to any AI agent and take full control of your property management system (PMS) and automated hostel/hotel operations through natural conversation.

### What you can do

- **Reservation Portfolio Orchestration** â€” List and manage all property reservations programmatically, retrieving detailed stay metadata and payment statuses
- **Guest & Customer Intelligence** â€” Programmatically retrieve directories of guests and access complete profiles and check-in history in real-time
- **Room & Inventory Architecture** â€” Access your complete directory of rooms and availability to coordinate your organizational resource allocation
- **Operational Monitoring** â€” Access real-time status updates for check-ins/outs and track property performance directly through your agent for instant reporting
- **Infrastructure Verification** â€” Verify account-level API connectivity and monitor booking volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your HQBeds dashboard (Settings > Integrations)
3. Start orchestrating your hospitality growth from Claude, Cursor, or any MCP client

No more manual checking of availability calendars or missing guest check-in times. Your AI acts as your dedicated front-desk coordinator and PMS architect.

### Who is this for?

- **Hostel & Hotel Managers** â€” instantly retrieve booking summaries and monitor occupancy using natural language commands
- **Reception Leads** â€” verify individual guest metadata and track payment history without leaving your creative workspace
- **Developers** â€” integrate high-speed HQBeds data into custom hospitality apps through simple AI queries


## Available Tools (10)
- **get_reservation**: Get reservation details
- **get_room**: Get room details
- **list_availability**: Use ISO 8601 dates.

Check room availability
- **list_guests**: List all guests
- **list_reservations**: List all reservations
- **list_rooms**: List all rooms
- **check_hqbeds_status**: Verify HQBeds API connectivity
- **create_reservation**: Create a reservation
- **get_account**: Get account info
- **get_guest**: Get guest details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HQBeds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reservations checking in today."

**🤖 AI Agent:**
> You have 5 arrivals today. The first is John Smith in Room 101 (2 nights, paid). Would you like to see guest details or payment status for any of them?

---

**👤 You:**
> "Show room availability for this weekend."

**🤖 AI Agent:**
> This weekend you have 85% occupancy. 3 rooms are still available: Room 205 (double), Room 308 (single), and Room 412 (suite). Would you like to create a reservation?

---

**👤 You:**
> "Create a reservation for Maria Silva, Room 205, checking in May 10 and out May 12."

**🤖 AI Agent:**
> Done! Reservation created for Maria Silva in Room 205, May 10-12 (2 nights). Confirmation ID: RSV-4821. Would you like to send a confirmation email to the guest?


## ❓ FAQ

**Q: How do I find my HQBeds API key?**
Log in to your HQBeds dashboard, navigate to **Settings > Integrations**, and copy your API key from the credentials section.

**Q: Can my AI agent check room availability?**
Absolutely. Use the `list_availability` tool to retrieve real-time availability across all rooms for any date range.

**Q: How do I create a new reservation?**
Use the `create_reservation` tool with guest name, room ID, check-in and check-out dates. Your agent handles the rest automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hqbeds](https://vinkius.com/mcp/hqbeds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HQBeds** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hqbeds` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HQBeds** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hqbeds": {
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
