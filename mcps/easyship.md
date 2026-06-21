# Easyship MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/easyship)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage global shipments, track packages, and request shipping rates via the Easyship API.

## Description
Integrate **Easyship**, the leading global shipping platform for e-commerce, directly into your AI workflow. Manage your cross-border shipments and carrier rates, track packages in real-time with detailed checkpoint logs, monitor available couriers and their service levels, and oversee your logistics operations using natural language.

### What you can do

- **Shipment Oversight** — List and retrieve detailed information and real-time status for all your global logistics shipments.
- **Rate Intelligence** — Request instant shipping quotes and estimated delivery times for various couriers based on parcel details.
- **Tracking Monitoring** — Monitor active shipments, resolving real-time transit statuses, courier events, and delivery receipts.
- **Carrier Management** — Access and monitor all available couriers and their specific service capability boundaries.

### How it works

1. Connect the Easyship integration to your AI assistant.
2. Authorize using your Easyship API Key (found in your account settings).
3. Orchestrate your global logistics and shipment tracking through intuitive conversation.

### Who is this for?

- **E-commerce Managers** — Quickly check global shipping rates and delivery statuses on the go.
- **Logistics Teams** — Monitor in-transit shipments and carrier performance via chat.
- **Customer Support** — Research specific tracking details and delivery events to assist customers instantly.


## Available Tools
- **get_easyship_account_metadata**: Retrieve metadata and limits for your Easyship account
- **quick_shipping_volume_audit**: Retrieve a high-level summary of shipment activity and success rates
- **get_shipment_details**: Get detailed information and tracking for a specific shipment
- **list_available_couriers**: List all available couriers and their service capability boundaries
- **list_failed_deliveries**: Identify shipments that have failed delivery or encountered issues (mock logic)
- **list_in_transit_shipments**: Identify shipments that are currently in transit with a courier
- **get_shipping_rates**: Request shipping rates for a potential shipment
- **list_latest_shipments**: Identify the most recently created or updated shipments
- **list_logistics_shipments**: List all shipments in your Easyship account
- **search_shipments_by_reference**: Search for shipments using a reference ID or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Easyship** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent global shipments."

**🤖 AI Agent:**
> I've found 5 recent shipments, including deliveries to Hong Kong and the United Kingdom. 2 are 'In Transit' and 3 are 'Delivered'. Would you like the tracking number for the Hong Kong shipment?

---

**👤 You:**
> "Get shipping rates from USA to France for a 1kg parcel."

**🤖 AI Agent:**
> I've retrieved 3 rates for this route: FedEx International Connect ($25.00, 5 days), UPS Worldwide Saver ($42.00, 2 days), and DHL Express ($38.00, 3 days). Would you like to see the full JSON parameters for these rates?

---

**👤 You:**
> "Check the status of shipment 'ES-12345678'."

**🤖 AI Agent:**
> Shipment 'ES-12345678' is currently 'In Transit'. The last checkpoint was 'Arrived at Sorting Facility' in Singapore. ETA is March 20th. Should I pull the full delivery history?


## ❓ FAQ

**Q: How do I get an Easyship API Key?**
Log in to your Easyship dashboard, navigate to **Connect > API**, and you can create a new API token or retrieve an existing one from there.

**Q: Can the agent generate labels?**
This integration currently focuses on listing and auditing shipments, tracking, and rates. Purchasing and printing shipping labels should be managed via the Easyship web portal or dedicated creation API endpoints.

**Q: Does it support international shipping?**
Yes, Easyship is designed specifically for global logistics. The agent can retrieve rates and tracking for both domestic and international shipments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easyship](https://vinkius.com/mcp/easyship)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Easyship** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `easyship` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Easyship** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "easyship": {
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
