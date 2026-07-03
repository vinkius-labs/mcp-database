# OpenCage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Geocode addresses and reverse-geocode coordinates via OpenCage — convert locations to lat/lng and back with country, language, and privacy filters from any AI agent.

## Description
Give your AI agent precise geolocation superpowers with **OpenCage Geocoding**. Convert any address into coordinates, reverse-geocode GPS pins into readable addresses, and apply advanced filters — all through natural conversation.

### What you can do

- **Forward Geocoding** — Convert any address or place name into exact latitude/longitude coordinates
- **Reverse Geocoding** — Turn GPS coordinates into structured street addresses with timezone and sun data
- **Country Filtering** — Restrict results to a specific country (ISO 3166-1 Alpha-2) to avoid ambiguous city matches
- **Language Bias** — Request results localized in any IETF language code (e.g., pt-BR, fr-FR)
- **Confidence Scoring** — Filter geocoding results by minimum confidence level (1–10) for delivery-grade accuracy
- **Bounding Box** — Constrain results to a geographic rectangle for targeted regional searches
- **Privacy Mode** — Run geocoding queries without OpenCage logging them, for sensitive addresses
- **Duplicate Control** — Return or suppress duplicate results for data validation workflows

### How it works

1. Subscribe to this server
2. Enter your OpenCage API Key
3. Start geocoding from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics teams** — validate delivery addresses before dispatching drivers to avoid failed deliveries
- **Data engineers** — enrich datasets with lat/lng coordinates and timezone metadata at scale
- **Privacy-conscious apps** — geocode sensitive addresses without leaving a trace in third-party logs


## Available Tools (10)
- **reverse_fetch_time_annotations**: Irreversibly vaporize explicit validation limits extracting UTC logic
- **geocode_basic**: Identify bounded routing spaces inside the Headless OpenCage Engine
- **geocode_bounding_box**: Inspect deep internal arrays mitigating specific Polygon domains
- **geocode_high_confidence**: Dispatch an automated validation check routing explicit Score limits
- **geocode_country_filter**: Perform structural extraction of properties driving active Country nodes
- **geocode_language_bias**: Retrieve explicit Cloud logging tracing explicit Payload locales
- **geocode_all_duplicate_results**: Retrieve the exact structural matching verifying Delivery alternatives
- **geocode_no_record_privacy**: Provision a highly-available JSON Payload generating secure mappings
- **reverse_basic**: Enumerate explicitly attached structured rules exporting active GPS pins
- **reverse_fast_no_annotations**: Identify precise active arrays spanning native Location limits faster


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the coordinates for 1600 Amphitheatre Parkway, Mountain View, CA?"

**🤖 AI Agent:**
> Found 1 result with confidence 10/10. Latitude: 37.4220, Longitude: -122.0841. Timezone: America/Los_Angeles (UTC-7). County: Santa Clara. The result is formatted as '1600 Amphitheatre Parkway, Mountain View, CA 94043, United States'. Want me to run this through a different language?

---

**👤 You:**
> "What's at coordinates 48.8566, 2.3522?"

**🤖 AI Agent:**
> Reverse geocoding result: Paris, Île-de-France, France. Formatted address: 'Rue de Rivoli, 75001 Paris, France'. Timezone: Europe/Paris (CET, UTC+1). Sunrise today: 07:12, Sunset: 19:45. Country code: FR. Want me to strip annotations for a faster, lighter response?

---

**👤 You:**
> "Geocode 'Springfield' but only show results in the United States with confidence >= 7."

**🤖 AI Agent:**
> Found 5 results in the US with confidence ≥ 7. Top match: Springfield, IL (confidence 9) — 39.7817, -89.6501 (state capital). Also: Springfield, MO (confidence 8), Springfield, MA (confidence 8), Springfield, OH (confidence 7), Springfield, OR (confidence 7). Want details on any of these?


## ❓ FAQ

**Q: How accurate is the geocoding — can I use it for delivery routing?**
OpenCage returns a confidence score from 1 to 10 for each result. Use the high-confidence filter (min_confidence=8 or higher) to get delivery-grade accuracy. Combined with country filtering, you can eliminate ambiguous matches and get coordinates reliable enough for last-mile dispatch.

**Q: What does privacy mode actually do?**
When you enable no_record=1, OpenCage processes your query but doesn't log it in their cache or analytics. The result is identical, but the query leaves no trace on their servers. Ideal for geocoding patient addresses, legal documents, or any PII-sensitive data.

**Q: Can I geocode in multiple languages — like getting results in Portuguese for a Brazilian address?**
Yes. Use the language bias tool with any IETF language code (pt-BR, es-MX, fr-FR, etc.) and OpenCage returns the address components translated to that locale. Perfect for building multilingual apps or standardizing address formats across regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencage](https://vinkius.com/mcp/opencage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opencage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencage": {
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
