# REST Countries MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rest-countries)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Manage your global research — audit country records, currencies, and languages via AI.

## Description
Empower your AI agent to orchestrate your entire global research workflow with **REST Countries**, the authoritative source for geographic and geopolitical data. By connecting REST Countries to your agent, you transform complex demographic searches into a natural conversation. Your agent can instantly search for countries, audit currency distributions, and retrieve language metadata without you ever touching a technical database. Whether you are conducting market expansion research or building global applications, your agent acts as a real-time geographic consultant, ensuring your data is always comprehensive and well-categorized.

### What you can do

- **Country Auditing** — Search for any country by its common or official name and retrieve detailed metadata, including capitals and population counts.
- **Regional Oversight** — Browse countries by region or subregion to maintain a clear view of global geographic distributions.
- **Economic Intelligence** — Query countries by currency to understand the reach of specific financial systems instantly.
- **Linguistic Discovery** — Retrieve lists of countries that speak specific languages to assist in localization planning.
- **Spatial Discovery** — Retrieve official flags and geographic coordinates for any country ID to maintain visual and spatial context.

### How it works

1. Subscribe to this server
2. No API Key required (REST Countries is a free and open service)
3. Start managing your global intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **International Researchers** — monitor geographic data and retrieve country metadata straight from your workflow.
- **Localization Managers** — verify language support and audit regional clusters without manual database exports.
- **Data Analysts** — perform rapid audits of demographic markers and identify currency zones through natural language.
- **Operations Leads** — automate global data querying to orchestrate cross-functional international teams smoothly.


## Available Tools (6)
- **get_all_countries**: Get a list of all countries in the world
- **get_countries_by_currency**: List countries that use a specific currency
- **get_countries_by_language**: List countries that speak a specific language
- **get_countries_by_region**: List countries in a specific region or subregion
- **get_country_by_code**: Search for a country by its ISO alpha-2 or alpha-3 code
- **get_country_by_name**: Search for a country by its common or official name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **REST Countries** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the country 'Brazil' using REST Countries."

**🤖 AI Agent:**
> I've retrieved the details for Brazil 🇧🇷. Its capital is Brasília and it has a population of over 212 million. Would you like to see the currencies or languages spoken?

---

**👤 You:**
> "List all countries in the region 'Europe'."

**🤖 AI Agent:**
> I've retrieved the list of countries in Europe. Notable entries include France, Germany, and Italy. I can provide the capital and flag for each if you'd like.

---

**👤 You:**
> "Which countries speak 'Spanish'?"

**🤖 AI Agent:**
> I've identified over 20 countries where Spanish is an official language, including Spain, Mexico, and Argentina. Would you like the population count for any specific one?


## ❓ FAQ

**Q: Is an API Key required for REST Countries?**
No. REST Countries is a free and open service. This server works out of the box without any static credentials required.

**Q: Can the agent search for countries by currency?**
Yes. Use the `get_countries_by_currency` tool providing the currency code (e.g., 'EUR'). Your agent will return all countries using that specific currency instantly.

**Q: Is population data included?**
Yes. Every country record retrieved by your agent includes the most recent official population count available in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rest-countries](https://vinkius.com/mcp/rest-countries)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **REST Countries** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rest-countries` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **REST Countries** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rest-countries": {
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
