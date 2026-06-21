# Navisphere MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/navisphere)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shipping-logistics](../categories/shipping-logistics.md)

Automate freight logistics via Navisphere — search available loads, submit bids, track shipments, and manage documentation directly from your AI agent.

## Description
Connect your **Navisphere** (C.H. Robinson) account to any AI agent to streamline your supply chain and freight operations through natural conversation.

### What you can do

- **Load Discovery** — Search for available freight loads by origin, destination, equipment type (V, R, F, VV), and pickup dates.
- **Bidding & Offers** — Submit pricing bids for specific loads and accept freight offers extended to your carrier account.
- **Shipment Management** — Create new shipments and update statuses (Arrived, Loaded, Departed) with precise location data.
- **Real-time Tracking** — Fetch the latest milestones, ETAs, and tracking events for any active shipment.
- **Digital Documentation** — Upload BOL, POD, and receipts directly to shipments to accelerate billing and compliance.
- **Rate Estimation** — Get instant spot market or contract rate estimates based on lane and equipment data.

### How it works

1. Subscribe to this server
2. Enter your Navisphere Client ID and Client Secret
3. Start managing your logistics pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Carriers & Dispatchers** — Find and bid on loads instantly without switching between multiple web portals.
- **Logistics Coordinators** — Update shipment statuses and upload proof of delivery (POD) via simple voice or text commands.
- **Supply Chain Managers** — Track high-priority shipments and get rate estimates for new lanes in seconds.


## Available Tools
- **accept_offer**: Accept a freight offer
- **create_shipment**: Create a new shipment (Customer API)
- **get_load_details**: Get details for a specific available load
- **get_rate_estimate**: Uses POST under the hood but acts as a query.

Get a rate estimate for a shipment
- **get_tracking_events**: Get high-frequency tracking events for a shipment
- **search_available_loads**: Search for available freight loads
- **submit_bid**: Submit a bid for an available load
- **subscribe_webhooks**: Subscribe to real-time visibility events
- **track_shipment**: Track a customer shipment
- **update_shipment_status**: g., Arrived, Loaded, Departed).

Update the status of an assigned shipment
- **upload_shipment_documents**: Upload documents for a shipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Navisphere** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for available loads from Chicago, IL to Dallas, TX for a Van (V)."

**🤖 AI Agent:**
> I found 3 available loads matching your criteria. The most relevant is Load #882910, picking up tomorrow with a weight of 42,000 lbs. Would you like the full details or to submit a bid?

---

**👤 You:**
> "Submit a bid of 1500 USD for load 882910. Contact is John Doe."

**🤖 AI Agent:**
> Bid successfully submitted! Your offer of $1,500 USD for Load #882910 has been recorded under John Doe. I will notify you if the status changes.

---

**👤 You:**
> "Track shipment ID 992288 and show me the latest ETA."

**🤖 AI Agent:**
> Shipment 992288 is currently 'In Transit'. The latest milestone was 'Departed Chicago Terminal' at 08:00 AM. The estimated arrival in Dallas is tomorrow at 04:30 PM.


## ❓ FAQ

**Q: How do I find available loads for a specific route and equipment type?**
Use the `search_available_loads` tool. You can filter by `originCity`, `destinationCity`, and `equipmentType` (e.g., 'V' for Van, 'R' for Reefer) to see all matching freight opportunities.

**Q: Can I update the location and status of a shipment while in transit?**
Yes! Use the `update_shipment_status` tool with the `shipmentId`. You can provide a JSON object containing the new status code (e.g., 'Arrived') and current GPS coordinates.

**Q: How do I submit a price bid for a load I found?**
Use the `submit_bid` tool. Provide the `loadNumber`, your `bidAmount`, the `currency`, and a `contactName`. The system will register your offer directly in the Navisphere ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/navisphere](https://vinkius.com/mcp/navisphere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Navisphere** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `navisphere` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Navisphere** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "navisphere": {
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
