# Amsterdam Events, Venues & Sport MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-events-venues-sport)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless access to Amsterdam's registered public events, licensed food & beverage businesses and sport facilities — events, horeca permits, sports fields and providers, no API key.

## Description
Amsterdam's event, venue and sport data, keyless, straight from the city's open-data platform. No credentials — the evenementen, horeca and sport services are public.

### What you can do
- **Search events** — the city's registered public events, filterable by title, start date and end date
- **Find horeca licenses** — food & beverage operating permits (exploitatievergunning), with permit status, category and address — bars, restaurants, terraces
- **List sport fields** — sports fields by sport function (e.g. football, hockey), park and surface
- **Find sport providers** — organisations offering sport, by name, postal code and town

### Who is this for
Agents planning around the city calendar, food & beverage and venue research, sports analytics and local business intelligence.


## Available Tools (4)
- **search_events**: Filter by title or by start/end date.

Search events and public installations registered in Amsterdam
- **find_horeca_licenses**: Filter by business name, postal code or address.

Find licensed food & beverage establishments in Amsterdam
- **list_sport_fields**: g. Golf, Voetbal), surface type, construction year, area, park name and polygon geometry (EPSG:28999). Filter by sport function or park name.

List sports fields and outdoor sport facilities
- **search_sport_providers**: Filter by provider name, postal code or town.

Search sports providers and facilities in Amsterdam


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Events, Venues & Sport** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find licensed bars in postal code 1015NR."

**🤖 AI Agent:**
> find_horeca_licenses filtered by postal code 1015NR returns the permit rows: permit name, category (e.g. cafe/restaurant), address, permit status (e.g. in force) and permit number.

---

**👤 You:**
> "List all sports fields in a park, for football."

**🤖 AI Agent:**
> list_sport_fields filtered by sport function (voetbal for football, hockey) and park name returns the field rows: field name, sport functions, park, surface type and location.

---

**👤 You:**
> "What public events are registered around a given date?"

**🤖 AI Agent:**
> search_events filtered by start/end date returns the event rows: title, start and end datetime, location, organiser and a short description for each registered event in that window.


## ❓ FAQ

**Q: Do I need an API key?**
No. The evenementen, horeca and sport services of the city's DSO open-data platform are public (OPENBAAR) and work without credentials.

**Q: What does the horeca data include?**
Horeca records are operating permits (exploitatievergunning) for food & beverage businesses: permit name, category (cafe, restaurant, terraces, etc.), address, permit number, status and issuance details. They are not opening-hours or menu data.

**Q: How current are the events?**
Events are those formally registered with the city (permits, registrations). Filter by start/end date to get what is around your window; the data is not a real-time ticketing feed.

**Q: Can I filter sports fields by sport type?**
Yes. list_sport_fields supports the sport function filter (e.g. voetbal for football, hockey) plus park and surface filters. The sport type field is a multi-valued array, so it is matched as a filter rather than a query.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-events-venues-sport](https://vinkius.com/en/ai-agent-connect/amsterdam-events-venues-sport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Events, Venues & Sport** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-events-venues-sport` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Events, Venues & Sport** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-events-venues-sport": {
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
