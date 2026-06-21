# Booking Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/booking-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage yacht charters via Booking Manager — track yachts, check availability, and manage bookings directly from any AI agent.

## Description
Connect your **Booking Manager (MMK Systems)** account to any AI agent and orchestrate your yacht charter and fleet management workflows through natural conversation.

### What you can do

- **Fleet Oversight** — List all available yachts and retrieve detailed metadata, including models, equipment, and photos.
- **Real-time Availability** — Check yacht availability for specific dates and locations instantly.
- **Price Quotation** — Calculate detailed quotes including taxes, discounts, and mandatory extras.
- **Booking Management** — List all reservations and options, and create new bookings directly from your workspace.
- **Network Discovery** — Access the directory of charter companies, marinas (bases), and available yacht extras.
- **Automated Offers** — Retrieve pre-calculated price offers based on your criteria.

### How it works

1. Subscribe to this server
2. Enter your Booking Manager API Key
3. Start managing your charter business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Charter Brokers** — quickly check availability and generate quotes for clients without manual searches.
- **Fleet Operators** — monitor bookings and yacht statuses straight from their workflow tools.
- **Travel Agents** — retrieve yacht details and automated offers using natural language.


## Available Tools
- **check_availability**: Check yacht availability for specific dates
- **create_booking**: Create a new reservation or option
- **get_extras**: List available extras for a yacht
- **get_offers**: Get automated price offers
- **get_prices**: Calculate prices and quotes for a yacht
- **get_yacht**: Get details of a specific yacht
- **list_bases**: List all charter bases (marinas)
- **list_bookings**: List all reservations and options
- **list_companies**: List yacht charter companies/operators
- **list_yachts**: List all available yachts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Booking Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all yachts available in Croatia for June 2024."

**🤖 AI Agent:**
> I've checked the availability for June in Croatia. I found 12 yachts, including 'Sun Odyssey 440' and 'Lagoon 450'. Would you like price quotes for any of these?

---

**👤 You:**
> "Show the full equipment list for yacht 102."

**🤖 AI Agent:**
> Yacht 102 (Bavaria 46) features: GPS Chartplotter, Autopilot, Bimini top, Inverter, and Webasto heating. It also includes 4 cabins and 3 heads.

---

**👤 You:**
> "Calculate a quote for yacht 105 from 2024-07-06 to 2024-07-13."

**🤖 AI Agent:**
> Retrieving prices... The total quote for those dates is €3,450.00. This includes a 10% Early Booking discount and mandatory transit log fee of €150.00.


## ❓ FAQ

**Q: Can I check if a specific yacht is available for next week?**
Yes! Use the `check_availability` tool with the start and end dates. Your agent will fetch the real-time availability status from the Booking Manager database.

**Q: How do I calculate a full price quote for a charter?**
Simply ask the agent to `get_prices` and provide the Yacht ID and the charter dates. It will return a breakdown including the base price, discounts, and any mandatory fees.

**Q: Can I see photos and equipment lists for the yachts?**
Yes. Use the `get_yacht` tool with the specific Yacht ID to retrieve its full technical specifications, equipment details, and image links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/booking-manager](https://vinkius.com/mcp/booking-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Booking Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `booking-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Booking Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "booking-manager": {
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
