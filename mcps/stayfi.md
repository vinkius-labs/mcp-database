# StayFi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stayfi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Connect your AI agents to StayFi to capture guest emails, manage WiFi properties, monitor networks, and track marketing analytics.

## Description
Transform your vacation rental network into a powerful marketing engine by connecting your AI agents to StayFi. With 17 dedicated tools, your AI can automatically pull guest contact data, monitor router health, configure splash pages, and analyze email collection rates across your portfolio.

### What you can do
- Capture and export guest emails and phone numbers
- Manage vacation rental properties and networks
- Configure custom WiFi splash and login pages
- Monitor router health and online status in real-time
- Track email collection and marketing analytics
- Organize and segment guest lists for CRM integration

### How it works
1. Subscribe to this server
2. Enter your StayFi API Key (found in your provider dashboard)
3. Let your AI agents seamlessly manage your WiFi marketing via Vinkius

### Who is it for?
Tailor-made for vacation rental managers, boutique hoteliers, and hospitality operators looking to maximize direct bookings through captive portal data collection.


## Available Tools (17)
- **check_stayfi_status**: Verify connectivity
- **export_guests**: Export guest data
- **get_analytics**: Get analytics overview
- **get_device_status**: Get device status
- **get_email_stats**: Get email collection stats
- **get_guest**: Get guest details
- **get_network**: Get network details
- **get_property_stats**: Get property stats
- **get_property**: Get property details
- **get_splash_page**: Get splash page
- **list_devices**: List hardware devices
- **list_guests_by_property**: List guests by property
- **list_guests**: List all guests
- **list_networks**: List WiFi networks
- **list_properties**: List properties
- **list_splash_pages**: List splash pages
- **search_guests**: Search guests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StayFi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all guests captured via WiFi at our beach property this week."

**🤖 AI Agent:**
> I've fetched the guest list for 'Oceanview Villa'. You've captured 15 new guest profiles this week, including 15 emails and 12 phone numbers. Would you like me to export this list for your next email campaign?

---

**👤 You:**
> "Are all StayFi routers online and functioning correctly?"

**🤖 AI Agent:**
> Running a diagnostic check... 23 out of 24 routers are currently online and broadcasting. However, the router at 'Mountain Cabin' has been offline for 2 hours. Should I pull the troubleshooting details for that specific device?

---

**👤 You:**
> "What is our email collection rate across all properties for the current month?"

**🤖 AI Agent:**
> Fetching your collection stats... This month, your portfolio has collected 342 new emails with an average opt-in rate of 68% across all splash pages. 'Downtown Loft' is your highest-performing property with 85 new contacts.


## ❓ FAQ

**Q: How can my AI retrieve the list of guests who connected to the WiFi at a specific property?**
Simply use the `get_property_guests` tool providing the specific property ID. Your agent will instantly compile a list of all guests captured via the captive portal, including their names, emails, and phone numbers.

**Q: Can I automatically check if all my routers are online across my portfolio?**
Yes! Ask the agent to run the `check_router_health` action. It will scan all your StayFi routers in real-time and report back any offline devices, ensuring your guest networks are always functional.

**Q: Is it possible to track the total number of emails collected this month?**
Absolutely. By utilizing the `get_collection_stats` tool, your agent can instantly fetch the email collection analytics across all properties, giving you an immediate view of your marketing data growth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stayfi](https://vinkius.com/mcp/stayfi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StayFi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stayfi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StayFi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stayfi": {
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
