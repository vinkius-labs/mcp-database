# CarAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/carapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Search 66,000+ vehicles — find cars by year, make, model, trim with engine specs, transmission and pricing data.

## Description
Connect to **CarAPI** and explore the comprehensive vehicle database through natural conversation.

### What you can do

- **Vehicle Search** — Search 66,000+ vehicles from 1990 to today by year, make, model, trim
- **Filter by Specs** — Filter by body type, engine type, drive type and transmission
- **Makes & Models** — Browse all car manufacturers and their model lineups
- **Vehicle Details** — Get full specs including engine, transmission, fuel economy, MSRP and dimensions
- **Reference Data** — Access complete lists of body types, engine types, transmissions and drive types

### How it works

1. Subscribe to this server
2. Enter your CarAPI API Key
3. Start exploring vehicle data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Car Shoppers** — compare vehicles by specs, find models by manufacturer and discover engine options
- **Dealerships** — access comprehensive vehicle data for inventory management and customer queries
- **Developers** — integrate automotive data into apps, websites and comparison tools


## Available Tools (8)
- **get_bodies**: ).

Get list of all body types
- **get_drives**: Get list of all drive types
- **get_engines**: ).

Get list of all engine types
- **get_makes**: Optionally filter by year to get makes available in a specific year. Returns make names and IDs.

Get list of all car makes
- **get_models**: Optionally filter by year. Returns model names and IDs.

Get models for a specific car make
- **get_transmissions**: ).

Get list of all transmission types
- **get_vehicles**: Supports filtering by year, make, model, body type, engine type, drive type and transmission. Returns vehicle details including year, make, model, trim, body style, engine specs, transmission, drive type, fuel type and MSRP.

Search vehicles by year, make, model and more
- **get_years**: Returns year values for filtering vehicle searches.

Get list of all available years in the database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CarAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all electric SUVs from 2024."

**🤖 AI Agent:**
> Found 25 electric SUVs from 2024 including: Tesla Model Y, Ford Mustang Mach-E, Hyundai Ioniq 5, Kia EV6, Rivian R1S. Each with MSRP, range, battery size and charging specs.

---

**👤 You:**
> "What models does Toyota make?"

**🤖 AI Agent:**
> Toyota makes 30+ models including: Corolla, Camry, RAV4, Highlander, Tacoma, Tundra, Prius, 4Runner, Sienna, Crown. Available years range from 1990 to 2024.

---

**👤 You:**
> "Show me specs for the 2024 Honda Civic."

**🤖 AI Agent:**
> 2024 Honda Civic: Body: Sedan. Engine: 2.0L 4-cylinder (158 hp) or 1.5L Turbo (180 hp). Transmission: CVT or 6-speed manual. Drive: FWD. Fuel: 31/40 mpg city/highway. MSRP: $24,650 - $30,650.


## ❓ FAQ

**Q: How do I get a CarAPI key?**
Sign up at [**carapi.app**](https://carapi.app/) and get your API key from the dashboard. Free tier available with limited requests.

**Q: How many vehicles are in the database?**
The database includes 66,000+ vehicles from 1990 to current year, covering all major manufacturers and models sold in the US market.

**Q: Can I filter vehicles by engine type?**
Yes! Use get_vehicles with engine_type parameter to filter by gas, diesel, electric, hybrid and more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/carapi](https://vinkius.com/mcp/carapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CarAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CarAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carapi": {
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
