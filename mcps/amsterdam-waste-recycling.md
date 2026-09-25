# Amsterdam Waste & Recycling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-waste-recycling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless access to Amsterdam's official waste calendar, waste fractions, street containers, container types and recycling point weighings — the city's open-data platform, no API key.

## Description
Everything the city of Amsterdam publishes about household waste, in one keyless integration. Data comes straight from the city's official DSO open-data platform (api.data.amsterdam.nl) — no credentials, no rate limits to manage.

### What you can do
- **Waste calendar (afvalwijzer)** — for any Dutch postal code, the registered waste streams, collection days (e.g. "Dinsdag"), bring-out windows and collection area
- **Waste fractions** — the full list of streams the city collects (Restafval, Papier, GFT, Glas, …) with codes and calendar order
- **Street containers** — locate public waste containers per stream, owner and neighbourhood
- **Container types** — the reference list of container types and volumes
- **Recycling point weighings** — weigh-in records at city recycling points, by location and fee group

### Who is this for
People moving to or visiting Amsterdam who need to know how waste collection works at their address, circular-economy analysts, waste operators and any agent that reasons about municipal waste logistics.


## Available Tools (5)
- **get_waste_calendar**: Fields are projected to keep the payload small. Some entries have empty instruction fields — that is how the city publishes them; rely on the stream name, collection days and collection area instead.

Waste collection calendar for an Amsterdam address (afvalwijzer)
- **list_waste_fractions**: Use it to learn the exact stream names and codes that can be passed to get_waste_calendar.

List the waste fractions (fracties) the city of Amsterdam collects
- **list_container_types**: A small reference list.

List the waste container types the city uses
- **find_waste_containers**: Useful for finding where a certain waste stream can be deposited.

Find public waste containers on Amsterdam streets
- **get_recycling_weighings**: Useful for checking which recycling points exist and what waste they weigh.

Get weigh-in records at city recycling points


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Waste & Recycling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the waste calendar for 1015NR, Eerste Anjeliersdwarsstraat 1?"

**🤖 AI Agent:**
> 🗑️ **Waste calendar for 1015NR**

Returns the waste streams registered for that address, each with its collection days (afvalwijzerOphaaldagen), bring-out window, instruction text and collection area (afvalwijzerInzamelgebiedNaam/Code). Streams include e.g. Glas and Restafval.

---

**👤 You:**
> "List all waste fractions the city collects and their codes."

**🤖 AI Agent:**
> The city collects several household streams — e.g. Restafval (Residueel), Papier, GFT, Glas and plastic streams — each with a code, an active flag and a calendar order, ready to filter the waste calendar by.

---

**👤 You:**
> "Where can I drop off paper in Amsterdam? Find paper waste containers."

**🤖 AI Agent:**
> 📦 **Paper containers**

Street containers registered for the Papier stream, each with its serial number, owner, status, location (neighbourhood id, public-space id) and polygon geometry in EPSG:28999.


## ❓ FAQ

**Q: Do I need an API key?**
No. All endpoints of the city's DSO open-data platform used by this integration are public (OPENBAAR) and work with zero credentials. The city has announced it may introduce a free key regime in the future; today the APIs are keyless.

**Q: Where does the data come from?**
From the city of Amsterdam's official open-data platform (api.data.amsterdam.nl/v1): the afvalwijzer (waste calendar), huishoudelijkafval v2 (fractions, containers, container types) and recyclepunten (recycling point weighings) dataset services.

**Q: Does the waste calendar return exact pickup dates?**
It returns the collection days registered per address and waste stream (e.g. "Dinsdag" = Tuesday) plus the bring-out window and collection area. The city publishes calendar schedules per stream rather than a per-house date, so treat the days-of-week as the collection schedule for that address.

**Q: Which areas are covered?**
All of the city of Amsterdam. The waste calendar is registered per address (postal code + street + house number); containers and recycling points carry their own location data, including EPSG:28999 (RD New) coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-waste-recycling](https://vinkius.com/en/ai-agent-connect/amsterdam-waste-recycling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Waste & Recycling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-waste-recycling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Waste & Recycling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-waste-recycling": {
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
