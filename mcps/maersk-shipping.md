# Maersk Shipping MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/maersk-shipping)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Maersk container shipping APIs as an MCP: shipment tracking by container/waybill, waybill document lookup, ocean products, locations, vessel schedules, port calls and deadlines — api.maersk.com with Basic/Bearer integration auth.

## Description
**Maersk — the world's largest container line** — and its official Integration Hub APIs as a single MCP server.

### What you can do
- **Track shipments** — live milestones (gate-in, loaded, discharged, gate-out), current positions and ETAs by container number, bill of lading or your own reference
- **Waybill lookup** — the classic document lookup by carrier SCAC (MAEU) + waybill number: parties, ports, containers
- **Ocean products** — bookable sailings between two locations with vessels, transit times and schedules
- **Vessels & port calls** — vessel metadata, IMONumber schedules, arrival/departure records per port
- **Deadlines** — documentation, VGM, gate-in, demurrage and detention cut-offs per shipment

### Authentication (from the Maersk Integration Hub)
1. Create an account at **developer.maersk.com** (the 'Maersk Integration Hub')
2. Create an **app/integration** and subscribe it to the products you need (Shipment Tracking, Shipping Documents, Ocean Products, Vessel Schedules, Port Calls, Deadlines)
3. Copy the issued **Consumer Key + Consumer Secret** (and optionally a pre-minted Bearer token and your customer code) into this MCP's credentials

The gateway (api.maersk.com) accepts HTTP **Basic** (consumer key:secret) or **Bearer** tokens; every unauthenticated call returns a structured 401 with a `correlationIdentifier` for Maersk support.

### Who is this for?
Shippers and freight forwarders, supply-chain dashboards, logistics developers, e-commerce ops and AI agents that need authoritative Maersk ocean-freight data.


## Available Tools (7)
- **find_waybill**: json?carrierSCAC=MAEU&waybillNumber=... — returns the waybill metadata for MAEU (Maersk) bills: parties, ports, containers. carrierSCAC is the standard carrier code (MAEU for Maersk Line).

Look up a shipment by Bill of Lading (waybill) number — the classic Maersk document lookup
- **search_locations**: Search Maersk location master data: cities, ports, terminals (geo IDs)
- **get_deadlines**: Filter by waybillNumber or containerNumber. Requires the Deadlines subscription.

Get shipment deadlines: documentation, VGM, demurrage/detention cut-offs
- **track_shipments**: Query by containerNumber (e.g. MAEU1234567), waybillNumber or your reference. Requires the Shipment Tracking subscription.

Track shipments by container number, waybill number or your own reference (live milestones)
- **get_ocean_products**: ), numberOfTwentyEq / numberOfFortyEq. Returns sailings with vessels, transit times and deadlines. Requires the Ocean Products subscription.

Search bookable ocean products (sailings) between two locations with prices
- **get_vessel_schedules**: — vessel metadata and sailing schedules. Use IMONumber (7 digits) from prior calls; omit filters to list vessels within your subscription scope.

Get vessel schedules and routes for Maersk vessels (IMONumber)
- **get_port_calls**: Filter by vesselIMONumber (7 digits) and optionally port UN/LOCODE. Requires the Port Calls subscription.

Get port call records for a vessel (arrivals, departures, terminals)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maersk Shipping** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is container MAEU1234567 right now?"

**🤖 AI Agent:**
> 🚢 **Tracking MAEU1234567**

Current: discharged at Rotterdam, final destination Copenhagen
Milestones: gate-in Shenzhen 2026-08-02 → loaded 08-05 → discharged RTM 09-04 → gate-out pending
ETA Copenhagen: 2026-09-10

Want the full milestone list or the waybill document?

---

**👤 You:**
> "Find the waybill MAEU123456789 and its parties"

**🤖 AI Agent:**
> 📄 **Waybill MAEU123456789 (SCAC MAEU)**

Shipper: Nordic Exports AB · Consignee: BR Comércio Ltda
Port of loading: Gteborg (SEGOT) → Discharge: Santos (BRSSZ)
Containers: 2× 40HC

Full parties, ports and container list pulled from /v1/waybills/find.json.

---

**👤 You:**
> "Ocean products from Rotterdam to Santos departing next week"

**🤖 AI Agent:**
> ⛵ **Ocean products RTM→SSZ**

GeoIDs resolved via search_locations. Next sailings:
- Maersk Sentosa, dep 2026-09-12, transit 18d, direct
- Maersk Yellowstone, dep 2026-09-14, transit 21d, 1 transhipment

Deadlines per sailing (doc/VGM cut-offs) included. Want spot prices for a specific departure?


## ❓ FAQ

**Q: How do I get the Consumer Key/Secret?**
Create an account at developer.maersk.com (Maersk Integration Hub), create an app/integration in the catalogue, and subscribe it to the products you need (Shipment Tracking, Shipping Documents, Ocean Products, Vessel Schedules, Port Calls, Deadlines). The portal issues a Consumer Key + Consumer Secret pair per app.

**Q: I get a 401 with a correlationIdentifier — what now?**
The gateway returns a structured 401 (with httpMethod, requestUri and correlationIdentifier) whenever auth is missing/invalid — first check the consumer key/secret. Maersk support can trace any request by that correlation identifier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/maersk-shipping](https://vinkius.com/en/ai-agent-connect/maersk-shipping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maersk Shipping** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maersk-shipping` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maersk Shipping** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maersk-shipping": {
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
