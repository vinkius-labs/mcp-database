# Moova MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moova)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate smart logistics via Moova — create shipments, track deliveries, get shipping quotes, and orchestrate carriers from any AI agent.

## Description
Connect your **Moova** B2B logistics account to any AI agent and orchestrate your entire delivery operation through natural conversation.

### What you can do

- **Shipment Management** — Create, update, and cancel delivery orders with full origin/destination address details and contact information
- **Real-time Tracking** — Follow every shipment through GPS-powered tracking events including carrier handoffs, delivery attempts, and proof of delivery
- **Smart Quoting** — Get instant shipping cost estimates between any two addresses using Moova's intelligent carrier routing engine
- **Label Generation** — Download printable shipping labels with barcodes and QR codes for any registered shipment
- **Coverage Intelligence** — Query available delivery zones across Argentina and Latin America before committing to an order
- **Webhook Automation** — Configure real-time notifications for shipment status changes to keep your systems synchronized

### How it works

1. Subscribe to this server
2. Enter your Moova App ID and App Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated logistics coordinator, eliminating manual order entry and constant dashboard monitoring.

### Who is this for?

- **E-commerce Operations** — automate shipment creation from order data and monitor delivery progress without a separate logistics dashboard
- **Logistics Managers** — track fleet-wide delivery status and generate cost estimates for sales teams in real-time
- **Customer Support** — instantly pull tracking information and shipment status to respond to delivery inquiries within seconds


## Available Tools (14)
- **cancel_shipment**: Once cancelled, the shipment cannot be reactivated and a new one must be created if needed.

Cancel an active shipment order
- **create_shipment**: Requires origin and destination addresses with full street details, contact information, and package dimensions. Moova will automatically assign the optimal carrier and route based on real-time availability.

Create a new logistics shipment
- **create_webhook**: Essential for keeping your e-commerce platform synchronized with delivery progress.

Register a new webhook for shipment events
- **delete_webhook**: Remove a webhook endpoint
- **get_account_info**: Get merchant account information
- **get_budget**: Returns pricing from available carriers including express, same-day, and standard delivery options.

Get a shipping cost estimate
- **get_shipment_label**: The label includes barcode, QR code, and all routing information required by the assigned carrier.

Download the shipping label for a shipment
- **get_shipment_status**: Get the current status of a shipment
- **get_shipment**: Get full details of a specific shipment
- **list_coverage_zones**: List all available delivery coverage zones
- **list_shipments**: Can be filtered by shipment status (e.g., CREATED, IN_TRANSIT, DELIVERED, CANCELLED) to narrow results.

List all shipments with optional status filter
- **list_webhooks**: List all registered webhooks
- **track_shipment**: Get real-time tracking events for a shipment
- **update_shipment**: Changes are not allowed after the carrier has collected the package.

Update shipment details before pickup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moova** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a delivery from 'Av. Corrientes 1234, Buenos Aires' to 'Av. Santa Fe 5678, Buenos Aires' for Juan Pérez."

**🤖 AI Agent:**
> Shipment created successfully! ID: MOV-28491-AR. Moova assigned carrier 'Flash Express' with an estimated delivery window of 3-5 hours. The printable label is ready — shall I retrieve it for you?

---

**👤 You:**
> "How much would it cost to ship from Palermo to Belgrano in Buenos Aires?"

**🤖 AI Agent:**
> I've calculated the shipping estimates. Same-day delivery via Flash Express: $1,250 ARS. Next-day delivery via Correo Argentino: $780 ARS. Standard 2-day via Moova Economy: $520 ARS. Shall I create a shipment with any of these options?

---

**👤 You:**
> "Track my shipment MOV-28491-AR and tell me where it is right now."

**🤖 AI Agent:**
> Tracking shipment MOV-28491-AR... Current status: IN_TRANSIT. The package was picked up at 14:32 from Av. Corrientes 1234 and is currently en route with driver Martín G. (Flash Express). Last GPS ping: Av. Cabildo y Juramento at 15:10. Estimated delivery: 16:00-17:00 today.


## ❓ FAQ

**Q: Can my AI agent get an instant shipping quote between two addresses in Argentina?**
Yes! Use the `get_budget` tool with the origin and destination addresses. Moova's smart routing engine will return pricing from all available carriers including same-day, next-day, and standard delivery options.

**Q: How do I track a shipment in real-time and see all delivery events?**
Ask the agent to run `track_shipment` with your shipment ID. You'll receive a chronological list of all tracking events with GPS coordinates, timestamps, and carrier notes — from pickup to final delivery confirmation.

**Q: Can I cancel a shipment that hasn't been picked up yet?**
Yes. Use the `cancel_shipment` tool with the shipment ID. Cancellation is only possible before the carrier picks up the package. Once picked up, the shipment must complete its delivery cycle. A new shipment will need to be created if needed afterward.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moova](https://vinkius.com/mcp/moova)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moova** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moova` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moova** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moova": {
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
