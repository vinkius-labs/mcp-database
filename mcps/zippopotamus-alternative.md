# Zippopotam.us MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zippopotamus-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Free geocoding and postal code lookup — retrieve city, state, and coordinates for any zip code or find postal codes by city.

## Description
Connect to **Zippopotam.us** to empower your AI agent with global geocoding and postal code intelligence. This integration provides instant access to location data for dozens of countries, making it easy to resolve addresses and coordinates through natural conversation.

### What you can do

- **Postal Code Intelligence** — Retrieve city, state, and precise GPS coordinates (latitude and longitude) for any valid postal code using `get_location_by_postal_code`.
- **City Mapping** — Query all postal codes associated with a specific city and state/province to understand regional coverage via `get_postal_codes_by_city`.
- **International Support** — Access geographic data across multiple countries (US, DE, FR, BR, etc.) using standard ISO 3166-1 alpha-2 codes.
- **Data Enrichment** — Automatically fill in missing geographic metadata in your workflows or datasets without complex GIS software.

### How it works

1. Subscribe to this server
2. Enter 'PUBLIC' as your access key (no registration required for this public API)
3. Start querying location data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — verify zip codes and fetch coordinates for mapping components without leaving the code editor.
- **Data Scientists** — clean and enrich address datasets with standardized city and state information.
- **Logistics & E-commerce** — validate shipping destinations and calculate regional routing based on postal codes.


## Available Tools
- **get_location_by_postal_code**: Get location information by postal code
- **get_postal_codes_by_city**: Get postal codes by city and state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zippopotam.us** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the location details for US postal code 90210."

**🤖 AI Agent:**
> I've retrieved the data for zip code 90210. It is located in Beverly Hills, California (CA), United States. The coordinates are 34.0901 latitude and -118.4065 longitude.

---

**👤 You:**
> "List all postal codes for Seattle, Washington in the US."

**🤖 AI Agent:**
> Searching for Seattle, WA... I found multiple postal codes including 98101, 98102, 98103, 98104, and several others. Would you like the full list or details for a specific one?

---

**👤 You:**
> "What is the city and state for the German postal code 10115?"

**🤖 AI Agent:**
> The German postal code 10115 corresponds to the city of Berlin in the state of Berlin (BE).


## ❓ FAQ

**Q: How can I find the latitude and longitude for a specific zip code?**
Use the `get_location_by_postal_code` tool. Provide the country code (e.g., 'us') and the postal code. The agent will return the city, state, and precise GPS coordinates.

**Q: Can I find all postal codes for a specific city?**
Yes. Use the `get_postal_codes_by_city` tool. You will need to provide the country, the state abbreviation (e.g., 'ca' for California), and the city name.

**Q: What format should I use for the country parameter?**
The API requires ISO 3166-1 alpha-2 country codes. For example, use 'us' for the United States, 'de' for Germany, 'fr' for France, or 'br' for Brazil.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zippopotamus-alternative](https://vinkius.com/mcp/zippopotamus-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zippopotam.us** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zippopotamus-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zippopotam.us** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zippopotamus-alternative": {
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
