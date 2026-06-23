# J&T Express Malaysia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jt-express-malaysia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Orchestrate J&T Express Malaysia logistics — track parcels, manage orders, and calculate shipping directly from any AI agent.

## Description
Connect your AI agents to **J&T Express Malaysia**, the leading technology-driven logistics provider. This MCP provides 10 tools to automate real-time parcel tracking, manage shipment orders, and retrieve pricing information directly through natural conversation.

### What you can do

- **Logistics Orchestration** — Track multiple parcels and retrieve granular status updates and historical events
- **Order Management** — Create, cancel, and retrieve shipment orders programmatically using the official VIP system
- **Shipping Intelligence** — Calculate delivery prices and monitor service availability between regions
- **Waybill Processing** — Generate and retrieve waybill labels and metadata for authorized shipments
- **Regional Insights** — Verify city and postal code coverage for the Malaysian logistics network

### How it works

1. Subscribe to this server
2. Log in to the [**J&T Express VIP Portal**](https://vip.jtexpress.my/)
3. Navigate to **API Management** to obtain your **Customer Code** and **Password**
4. Identify your **API URL** (Production or Sandbox)
5. Insert your credentials into the fields below to start managing your Malaysian logistics.

### Who is this for?

- **E-commerce Developers** — automate the integration of J&T shipping and tracking into Malaysian storefronts
- **Fleet & Operations Managers** — monitor large volumes of outbound parcels via natural language
- **Customer Support Teams** — quickly provide real-time parcel statuses and shipping estimates


## Available Tools (10)
- **cancel_order**: Cancel a previously created delivery order
- **create_order**: Create a new J&T Express delivery order
- **get_order_details**: Get details for a specific order
- **get_shipping_rates**: Calculate estimated shipping costs
- **get_waybill_image**: Get the waybill label image link
- **list_area_codes**: Retrieve J&T internal area codes
- **list_cities**: List cities within a state
- **list_districts**: List districts within a city
- **list_provinces**: List all Malaysian states/provinces
- **track_order**: Track one or more shipments by bill code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **J&T Express Malaysia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track J&T parcel 'JT999888777' and show its current location."

**🤖 AI Agent:**
> Connecting to J&T tracking service... Parcel 'JT999888777' is currently 'In Transit' and was last scanned at the Subang Jaya Distribution Center today at 10:15 AM. Would you like to see the full event history?

---

**👤 You:**
> "List all active shipment orders in my J&T VIP account."

**🤖 AI Agent:**
> Retrieving orders from J&T VIP... I've found 5 active shipment orders. 3 are 'Pending Pickup' and 2 are 'Awaiting Payment'. Which one would you like to inspect?

---

**👤 You:**
> "Check if J&T express provides delivery service to postal code '50450'."

**🤖 AI Agent:**
> Searching J&T network coverage... Yes! Postal code 50450 (Kuala Lumpur) is fully covered by J&T Express Malaysia. Both standard and express delivery services are available for this area.


## ❓ FAQ

**Q: Can I automatically track a J&T parcel just by providing the tracking number?**
Yes! Use the `track_parcel` tool with the tracking number (e.g., 'JT123456789'). Your agent will retrieve the current status, location, and the full history of logistics events from the J&T system.

**Q: How do I calculate shipping prices between two Malaysian cities?**
Use the `calculate_shipping` tool with the origin and destination city names or postal codes. The agent will return the estimated price based on J&T's standard rates.

**Q: Can I retrieve the waybill image for an existing order?**
Yes! Use the `get_waybill` tool with the Order ID. Your agent will retrieve the metadata and the URL to download or print the official waybill label.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jt-express-malaysia](https://vinkius.com/mcp/jt-express-malaysia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **J&T Express Malaysia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jt-express-malaysia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **J&T Express Malaysia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jt-express-malaysia": {
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
