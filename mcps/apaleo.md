# Apaleo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apaleo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage hotel reservations, properties, rooms, rate plans, folios, invoices, and availability for your Apaleo PMS through natural conversation.

## Description
Connect your **Apaleo** hotel to any AI agent — the API-first PMS built for modern hospitality.

### What you can do

- **Reservations** — Browse, filter by status, and view complete booking details
- **Properties** — Multi-property management with full configuration access
- **Rooms** — Room inventory with status, condition, and maintenance tracking
- **Rate Plans** — All pricing plans, restrictions, and availability rules
- **Finance** — Guest folios, charges, payments, and finalized invoices
- **Availability** — Sellable units calendar per room type and date range

### Who is this for?

- **Boutique Hotels** — Streamlined operations through conversational AI
- **Hotel Groups** — Multi-property dashboards and cross-portfolio analytics
- **Revenue Managers** — Rate plan optimization and availability management
- **Finance Teams** — Invoice tracking and folio reconciliation


## Available Tools
- **list_reservations**: The front-desk dashboard.

List hotel reservations
- **check_availability**: Shows sellable units per room type per day.

Check room availability
- **get_reservation**: Get reservation details
- **list_properties**: For multi-property hotel groups.

List hotel properties
- **get_property**: Get property details
- **list_room_types**: Standard, Deluxe, Suite, etc.

List room types
- **list_rooms**: List rooms
- **list_rate_plans**: List rate plans
- **list_folios**: Filter by reservation for guest billing.

List guest folios
- **list_invoices**: For accounting and audit.

List invoices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apaleo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all confirmed reservations arriving this week"

**🤖 AI Agent:**
> 🧊 **Confirmed Arrivals — This Week**

1. **Maria Santos** — Junior Suite
   📅 Oct 18 → Oct 21 (3 nights)
   💰 EUR 450.00 | BAR rate

2. **Thomas Müller** — Standard Double
   📅 Oct 19 → Oct 22 (3 nights)
   💰 EUR 285.00 | Corporate rate

3. **Sophie Laurent** — Deluxe King
   📅 Oct 20 → Oct 23 (3 nights)
   💰 EUR 525.00 | Package: B&B


## ❓ FAQ

**Q: What makes Apaleo different from other PMS?**
Apaleo is 100% API-first — every feature is accessible via REST API with OpenAPI/Swagger specs. It offers a free developer sandbox, OAuth 2.0, and a modular architecture where you pick the best tools for each function.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apaleo](https://vinkius.com/mcp/apaleo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apaleo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apaleo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apaleo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apaleo": {
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
