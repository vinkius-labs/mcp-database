# Amsterdam Addresses & Properties MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-addresses-properties)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Keyless access to Amsterdam's address register (BAG), buildings, property register (WOZ) and protected monuments — addresses, house numbers, building data and monument records, no API key.

## Description
Amsterdam's official address and property data, keyless. Built on the national registers the city maintains: the BAG address register, the buildings (panden) layer, the WOZ property register and the monuments register.

### What you can do
- **Find addresses** — registered address designations by postal code, house number and address type (BAG nummeraanduidingen)
- **Get one address** — full record by identificatie
- **Search buildings** — panden by name, dwelling type or location, with build year, floors and polygon geometry
- **Property register (WOZ)** — property records by WOZ object number, kind and use
- **Monuments** — protected monuments by name, address, type and status (Rijksmonument / Stadsmonument)

### Who is this for
Real-estate and geocoding agents, address validation, property research, heritage work and anyone building on top of Amsterdam's official address base.


## Available Tools (7)
- **find_monuments**: g. Pand), status (e.g. Rijksmonument, Stadsmonument), designation date, architects, original function and point geometry. Filter by name, address, status or type.

Find protected monuments in Amsterdam
- **find_addresses**: Filter by postal code and house number to locate one address.

Find registered addresses (BAG) in Amsterdam
- **get_address**: g. 0363200000006110): house number parts, postal code, address type, status, registration date and validity period.

Get one address designation by id
- **search_buildings**: g. Woning), location classification, original build year, number of floors, status and polygon geometry (EPSG:28999). Filter by building name or dwelling type.

Search buildings (BAG panden) in Amsterdam
- **get_building**: g. 0363100012061164): name, dwelling type, build year, floors, status and polygon geometry.

Get one building record by id
- **list_property_records**: g. Winkel, Woning, Kantoor) and use classification, with validity periods. Filter by WOZ object number to look up one property.

List property register records (WOZ)
- **get_monument**: g. 000e8f55-1d82-4d94-8f1f-5ca11b4d28cf): all details including public description, geometry and complex membership.

Get one monument record by id


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Addresses & Properties** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the registered address for 1015NR, house number 1."

**🤖 AI Agent:**
> 📍 **Address lookup**

find_addresses filtered by postal code 1015NR and house number 1 returns the address designation: house number parts (1, letter H), postal code, address type (e.g. Hoofdadres), status and registration date.

---

**👤 You:**
> "Is Tweede Weteringdwarsstraat 71 a protected monument?"

**🤖 AI Agent:**
> find_monuments filtered by that address returns the monument record: monument number, type (Pand), status (e.g. Rijksmonument), designation date and public description.

---

**👤 You:**
> "What kind of property is WOZ object 036300000001?"

**🤖 AI Agent:**
> list_property_records filtered by WOZ object number returns the register record: object kind (e.g. Winkel = shop), use classification (e.g. Niet-woning = non-residential) and validity period.


## ❓ FAQ

**Q: Do I need an API key?**
No. The bag, woz and monumenten services of the city's DSO open-data platform are public (OPENBAAR) and work without credentials.

**Q: What is the difference between BAG and WOZ?**
BAG is the national address register: it holds addresses (nummeraanduidingen), buildings (panden) and dwellings. WOZ is the property register: it holds valuation records per property object, with kind and use classifications. Use BAG to locate an address or building, WOZ to look up a property record.

**Q: What monument statuses are there?**
Monuments carry a status such as Rijksmonument (national monument) or Stadsmonument (city monument). find_monuments can filter by status, type (e.g. Pand), and also by under-review flag.

**Q: Are building geometries usable for mapping?**
Yes. Building (panden) records include polygon geometry in EPSG:28999 (RD New). Convert to WGS84 for plotting on standard world maps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-addresses-properties](https://vinkius.com/en/ai-agent-connect/amsterdam-addresses-properties)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Addresses & Properties** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-addresses-properties` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Addresses & Properties** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-addresses-properties": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
