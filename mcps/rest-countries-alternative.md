# REST Countries MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rest-countries-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access comprehensive global data including country names, capitals, currencies, and languages via the REST Countries API.

## Description
Connect your AI agent to the **REST Countries** database to retrieve instant, accurate information about any nation or territory in the world. This server provides a powerful interface to query geographic, economic, and political data through natural conversation.

### What you can do

- **Comprehensive Search** — Find countries by common or official names, capital cities, or international codes (ISO 3166-1).
- **Economic & Linguistic Data** — Query countries based on the currencies they use or the languages spoken by their citizens.
- **Regional Filtering** — Browse nations by continent (Region) or specific subregions to analyze geographic clusters.
- **Demographics & Identity** — Search by demonyms (what citizens are called) or check independence status.
- **Localized Results** — Search for countries using translated names in various languages.

### How it works

1. Subscribe to this server
2. Since this is a public API, no specific token is required (enter 'public' if prompted)
3. Start asking about world geography and country statistics in Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly gather country-level metadata for research and reporting
- **Developers** — verify ISO codes, currency formats, and language mappings without leaving the IDE
- **Educators & Students** — explore global facts and regional statistics through an interactive AI assistant


## Available Tools (12)
- **get_all_countries**: You MUST specify the fields you need (up to 10) to avoid 400 Bad Request.

Retrieve information about all countries
- **search_by_capital**: Search by capital city
- **search_by_code**: Search by country code
- **search_by_codes**: Search for multiple countries by their codes
- **search_by_currency**: Search by currency code or name
- **search_by_demonym**: Search by demonym
- **filter_by_independent**: Filter by independence status
- **search_by_language**: Search by language code or name
- **search_by_name**: Search by country name
- **filter_by_region**: g., Africa, Americas, Asia, Europe, Oceania).

Filter countries by region
- **filter_by_subregion**: g., Northern Europe, South America).

Filter countries by subregion
- **search_by_translation**: Search by translation name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **REST Countries** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the country named 'Brazil' and show its capital and population."

**🤖 AI Agent:**
> I found Brazil! Its capital is Brasília and it has a population of approximately 212 million people. Would you like to see its neighboring countries as well?

---

**👤 You:**
> "List all countries located in the 'South America' subregion."

**🤖 AI Agent:**
> I've filtered the data for South America. There are 12 independent countries and several territories in this subregion, including Argentina, Brazil, Chile, and Colombia. Do you need details on a specific one?

---

**👤 You:**
> "Which countries use the 'Japanese Yen' as their currency?"

**🤖 AI Agent:**
> The Japanese Yen (JPY) is the official currency of Japan. It is one of the most traded currencies in the world. Would you like to see more economic data for Japan?


## ❓ FAQ

**Q: How do I retrieve a list of all countries with specific data points?**
Use the `get_all_countries` tool. You must provide a comma-separated list in the `fields` parameter (e.g., 'name,capital,population') to specify exactly which information you want to receive.

**Q: Can I find countries based on the currency they use?**
Yes! Use the `search_by_currency` tool and provide the currency name or code (like 'euro' or 'USD'). The agent will return all countries where that currency is legal tender.

**Q: Is it possible to filter countries by their geographic region?**
Absolutely. Use the `filter_by_region` tool with values like 'Europe', 'Americas', 'Asia', 'Africa', or 'Oceania' to get a list of countries in that specific part of the world.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rest-countries-alternative](https://vinkius.com/mcp/rest-countries-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `rest-countries-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **REST Countries** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rest-countries-alternative": {
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
