# Clubspeed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clubspeed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage entertainment venues and bookings via Clubspeed — track customers, monitor reservations, and manage race heats directly from any AI agent.

## Description
Connect your **Clubspeed** account to any AI agent and take full control of your venue management and event reservations through natural conversation. Streamline how you manage racers, bookings, and activities natively.

### What you can do

- **Customer Oversight** — List and retrieve details for all registered customers (racers) including profiles and contact info natively
- **Reservation Intelligence** — Access and monitor all event reservations and bookings flawlessly
- **Activity Logistics** — List all activities available at your venue to manage scheduling securely
- **Race Management** — Access upcoming and past race heats and retrieve detailed performance metadata flawlessly
- **Waiver Auditing** — List and review signed liability waivers to ensure compliance securely
- **Venue Visibility** — Retrieve core account and venue information directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your Clubspeed Private Key and Site ID
3. Start managing your entertainment venue from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Venue Managers** — monitor daily bookings and customer volume using natural language
- **Event Coordinators** — audit reservation details and heat schedules without opening the dashboard
- **Support Teams** — quickly look up racer profiles and signed waivers straight from their chat interface
- **Ops Teams** — verify activity availability and monitor system health


## Available Tools
- **get_clubspeed_account_info**: Retrieve core account and venue information
- **get_customer_venue_details**: Get detailed information for a specific customer
- **get_reservation_details**: Get detailed information for a specific reservation
- **list_venue_activities**: List all activities available at the venue
- **list_venue_customers**: List all customers (racers) registered at the venue
- **list_race_heats**: List upcoming and past race heats
- **list_venue_reservations**: List all event reservations and bookings
- **list_customer_waivers**: List signed liability waivers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clubspeed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reservations for today in Clubspeed."

**🤖 AI Agent:**
> Retrieving today's reservations... I found 5 bookings: 'Birthday Party - Smith' (2:00 PM), 'Corporate Event - Acme' (4:30 PM), and 3 others. Would you like to see the racer counts for these?

---

**👤 You:**
> "Show me the details for customer ID '12345'."

**🤖 AI Agent:**
> Checking profile for customer 12345... This is John Doe (john@example.com). He has a valid waiver signed last month and has participated in 12 races total.

---

**👤 You:**
> "What are the upcoming race heats?"

**🤖 AI Agent:**
> Retrieving upcoming heats... You have 2 heats scheduled in the next hour: Heat #45 (Pro Karting) at 11:15 AM and Heat #46 (Junior Karting) at 11:30 AM.


## ❓ FAQ

**Q: Can I see if a customer has signed their waiver through the agent?**
Yes! Use the `list_customer_waivers` tool. The agent will return all signed waivers, allowing you to verify compliance before a customer starts their activity.

**Q: How do I check the race heat schedule for today?**
Use the `list_race_heats` tool. Your agent will fetch the list of upcoming and past heats, allowing you to monitor the day's schedule directly.

**Q: Where do I find my Clubspeed Private Key and Site ID?**
You can find your **Private Key** in your Clubspeed API settings. The **Site ID** is typically your account's subdomain (e.g., if your dashboard is `myvenue.clubspeed.com`, your Site ID is `myvenue`).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clubspeed](https://vinkius.com/mcp/clubspeed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clubspeed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clubspeed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clubspeed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clubspeed": {
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
