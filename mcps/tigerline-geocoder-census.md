# TIGER/Line Geocoder (Census) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tigerline-geocoder-census)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access official US Census Bureau geocoding services to convert addresses into coordinates and detailed census geography data.

## Description
Connect to the **US Census Bureau TIGER/Line Geocoder** to transform location data into actionable geographic insights directly within your AI agent.

### What you can do

- **Address Geocoding** — Convert single-line or structured addresses (street, city, state, zip) into precise latitude and longitude coordinates.
- **Census Geographies** — Retrieve high-resolution census data including tracts, blocks, and tribal areas for any location.
- **Puerto Rico Support** — Specialized geocoding for Puerto Rico addresses, including Urbanization and Municipio parameters.
- **Reverse Geocoding** — Submit coordinates to identify the exact census boundaries and administrative layers they fall within.
- **Batch Processing** — Process up to 10,000 addresses at once via CSV data for large-scale data analysis.
- **Benchmark Management** — List and select specific Census benchmarks and vintages to ensure data consistency across different time periods.

### How it works

1. Subscribe to this server
2. The service uses the public Census Bureau API (no complex registration required)
3. Start querying US geographic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — automate the mapping of addresses to census tracts for demographic analysis.
- **Urban Planners** — quickly identify administrative boundaries and census blocks for infrastructure projects.
- **Logistics Teams** — validate US addresses and normalize geographic data for routing and delivery.


## Available Tools (8)
- **batch_geocode_address**: Format: Unique ID, Street address, City, State, ZIP

Batch geocode up to 10,000 addresses
- **batch_geocode_coordinates**: Format: Unique ID, Longitude (X), Latitude (Y)

Batch lookup census geographies for coordinates
- **list_benchmarks**: g., Public_AR_Current) and their IDs.

List available Census Geocoder benchmarks
- **geocode_address_pr**: Geocode a structured Puerto Rico address
- **geocode_address**: Geocode a structured address
- **geocode_coordinates**: ) for a specific latitude and longitude.

Lookup census geographies for coordinates
- **geocode_oneline**: Geocode a single line address
- **list_vintages**: List available Census Geocoder vintages for a benchmark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TIGER/Line Geocoder (Census)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode the address '1600 Pennsylvania Ave NW, Washington, DC 20500' using the Public_AR_Current benchmark."

**🤖 AI Agent:**
> I've geocoded the address. The coordinates are Longitude: -77.03636, Latitude: 38.89715. This was matched using the Public_AR_Current benchmark.

---

**👤 You:**
> "What census tract and block are located at coordinates -76.9274, 38.8459?"

**🤖 AI Agent:**
> Checking census geographies... Those coordinates correspond to Census Tract 8007, Block 1004 in Prince George's County, Maryland (using the Current vintage).

---

**👤 You:**
> "List all available geocoding benchmarks."

**🤖 AI Agent:**
> I've retrieved the available benchmarks. You can use 'Public_AR_Current' (ID: 4), 'Public_AR_Census2020' (ID: 2020), or 'Public_AR_Census2010' (ID: 10) for your queries.


## ❓ FAQ

**Q: Can I get census tract and block information from a single address string?**
Yes! Use the `geocode_oneline` tool with `returntype` set to 'geographies'. Provide the address and a benchmark (like 'Public_AR_Current') to receive full geographic metadata.

**Q: How do I find out which census area a specific GPS coordinate belongs to?**
Use the `geocode_coordinates` tool. Input the longitude (x) and latitude (y) along with a benchmark and vintage. The agent will return the specific census layers for that point.

**Q: Does this server support geocoding for addresses in Puerto Rico?**
Yes, specifically via the `geocode_address_pr` tool. It includes fields for 'urb' (Urbanization) and 'municipio' which are essential for accurate Puerto Rico address matching.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tigerline-geocoder-census](https://vinkius.com/mcp/tigerline-geocoder-census)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TIGER/Line Geocoder (Census)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tigerline-geocoder-census` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TIGER/Line Geocoder (Census)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tigerline-geocoder-census": {
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
