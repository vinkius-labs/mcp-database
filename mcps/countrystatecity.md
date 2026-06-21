# CountryStateCity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/countrystatecity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access global geographic data — list countries, states, and cities with ISO codes and metadata directly from any AI agent.

## Description
Connect the **CountryStateCity** database to your AI agent and instantly retrieve accurate geographic data through natural conversation.

### What you can do

- **Global Country List** — Retrieve all countries with their ISO2/ISO3 codes, phone codes, and emojis
- **State & Province Discovery** — List all administrative divisions (states, provinces, regions) for any specific country
- **City Level Granularity** — Drill down into specific cities within a state or fetch all cities in a country (Supporter+ tier)
- **Detailed Metadata** — Access specific fields like latitude, longitude, and currency for precise location context

### How it works

1. Subscribe to this server
2. Enter your CountryStateCity API Key
3. Start querying global locations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly find ISO codes and regional IDs without leaving the code editor
- **Data Analysts** — validate geographic hierarchies and clean location data via chat
- **Logistics & E-commerce** — verify shipping regions and city-state relationships instantly


## Available Tools
- **get_country**: Get details for a specific country
- **get_state**: Get details for a specific state
- **list_cities_by_country**: Note: Requires Supporter+ tier.

List all cities within a specific country
- **list_cities_by_state**: List all cities within a specific state
- **list_countries**: List all countries
- **list_states**: List all states/provinces within a specific country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CountryStateCity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all countries and include their emojis."

**🤖 AI Agent:**
> I've retrieved the list of countries. Here are a few: Afghanistan (AF) 🇦🇫, Albania (AL) 🇦🇱, Algeria (DZ) 🇩🇿, and Andorra (AD) 🇦🇩. Would you like the full list or details for a specific one?

---

**👤 You:**
> "What are the states in India (IN)?"

**🤖 AI Agent:**
> Querying states for India... I found 36 states/territories, including Maharashtra (MH), Delhi (DL), Karnataka (KA), and Tamil Nadu (TN). Which state would you like to explore further?

---

**👤 You:**
> "List the cities in the state of New York (NY), US."

**🤖 AI Agent:**
> Fetching cities for New York, United States... I've found cities such as Albany, Buffalo, New York City, and Rochester. Do you need specific details for any of these cities?


## ❓ FAQ

**Q: How can I list all cities within a specific state or province?**
Use the `list_cities_by_state` tool by providing the Country ISO2 code (e.g., 'US') and the State ISO2 code (e.g., 'NY'). The agent will return a list of all cities registered in that region.

**Q: Can I get detailed metadata like emojis and phone codes for a country?**
Yes! The `get_country` tool allows you to fetch full details for a specific country using its ISO2 code. You can also use `list_countries` with the `fields` parameter to include 'emoji' or 'phonecode' in the results.

**Q: Is there a limit when listing all cities in a country?**
The `list_cities_by_country` tool requires a Supporter+ tier API key from CountryStateCity. For standard users, it is recommended to use `list_cities_by_state` to query cities in smaller administrative batches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/countrystatecity](https://vinkius.com/mcp/countrystatecity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CountryStateCity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `countrystatecity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CountryStateCity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "countrystatecity": {
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
