# Air France-KLM Flights MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/air-france-klm-flights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Air France-KLM official Open Data APIs: live flight status by route or airport (AF/KL network, delays, gates) and commercial offers search with prices — apikey auth via the AFKL Developer Portal.

## Description
The **official Air France-KLM Open Data APIs** as a single MCP server — operational flight data from the AF/KL group, straight from the airline's own gateway.

### What you can do
- **Flight status by route** — AF1234, KL1000... for a specific date: operational status, departure/arrival airports and terminals, actual times, aircraft sub-family
- **Airport boards** — every AF/KL departure or arrival at an airport (AMS, CDG, LIS...) for a date
- **Latest schema** — v3 and v4 status endpoints both available
- **Commercial offers** — search fares and flight combinations between city pairs with cabin and passenger counts

### Authentication (from the AFKL Developer Portal)
1. Register at **developer.airfranceklm.com** (free account)
2. Create an app and subscribe it to the **Open Data APIs** (Flight Status and/or Commercial Offers)
3. Copy the generated **apikey** into this MCP's credentials — it is sent as the `apikey` HTTP header on every call

Without an active subscription the gateway answers `403 Developer Inactive`; a wrong path answers `596 Service Not Found` — so credential and path problems are always distinguishable.

### Who is this for?
Travel apps, flight-watch agents, ops dashboards, aviation analysts and anyone building on AF/KL operational data.


## Available Tools (4)
- **get_flight_status_by_airport**: Combine both origin and destination to narrow to a route.

Get all AF/KL flights departing/arriving an airport on a date (airport board)
- **get_flight_status_version4**: g. additional operational codes). Compare v3 vs v4 outputs if unsure which version your key covers.

Get flight status using the v4 endpoint (newest response schema)
- **search_offers**: Returns fare families, prices and flight combinations. Requires the Commercial Offers subscription on your AFKL key.

Search AF/KL commercial flight offers (prices, cabins) via the offers API
- **get_flight_status_by_route**: g. "AF1234", "KL1000", "KL0602") and scheduledDate (YYYY-MM-DD). Returns operational status (on time/delayed/cancelled), departure/arrival airports and terminals, actual times and aircraft sub-family. Requires an active Open Data subscription on the AFKL Developer Portal.

Get AF/KL flight status for a route number and date (delays, gates, equipment)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Air France-KLM Flights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is KL1000 on time today?"

**🤖 AI Agent:**
> ✈️ **KL1000 — 2026-09-07 (AF/KL Open Data)**

Route: Amsterdam (AMS) → Lisbon (LIS)
Status: Departed on time, 10:15 CEST
Arrival: 12:02 WEST (estimated on schedule)
Aircraft: Boeing 737-800 (KLM sub-family)

Want tomorrow's status or the return flight KL1001?

---

**👤 You:**
> "Which AF/KL flights leave Amsterdam tomorrow morning?"

**🤖 AI Agent:**
> 🛫 **AMS departures board (AF/KL network)**

Morning departures include:
- KL1001 AMS→LIS 06:00
- AF1741 AMS→CDG 07:15
- KL0613 AMS→NBO 10:00

All statuses pulled from the flightstatus endpoint with origin=AMS. Want arrivals instead, or only intercontinental routes?

---

**👤 You:**
> "Fares for AMS to JFK next Friday, 2 adults business class"

**🤖 AI Agent:**
> 💰 **AMS→JFK offers (AF/KL Commercial Offers)**

Business class, 2 adults, direct flights:
- KL0643 09:30→12:15 — from €2,840 pp
- KL0645 18:00→20:45 — from €2,610 pp

Both include full flat-bed cabins. Want economy comparison or the return-leg prices?


## ❓ FAQ

**Q: How do I get the apikey?**
Register free at developer.airfranceklm.com, create an app, and subscribe it to the Open Data APIs (Flight Status, Commercial Offers). The portal issues an apikey that is sent as the 'apikey' HTTP header. The Free tier has daily request limits; higher tiers need a paid subscription with AF/KL.

**Q: I get 403 'Developer Inactive' — what does it mean?**
The path exists but your apikey is inactive or not subscribed to that product. Check that the app subscription is active in the portal and that the key was copied fully. (A wrong path would instead return 596 'Service Not Found'.)


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/air-france-klm-flights](https://vinkius.com/en/ai-agent-connect/air-france-klm-flights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Air France-KLM Flights** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `air-france-klm-flights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Air France-KLM Flights** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "air-france-klm-flights": {
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
