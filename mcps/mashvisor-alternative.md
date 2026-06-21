# Mashvisor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mashvisor-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access real estate data, property search, and investment analytics — analyze rental rates, ownership info, and market performance via AI.

## Description
Connect your **Mashvisor** account to any AI agent to transform how you analyze real estate markets. Access professional-grade data for residential properties, Airbnb analytics, and investment performance metrics through natural conversation.

### What you can do

- **Property Search & Profiles** — Search for properties with specific filters and retrieve full profiles including tax history, transaction records, and Mashvisor AVM.
- **Investment Analysis** — Get historical performance, rental rates, and investment performance metrics for specific cities and neighborhoods.
- **Market Intelligence** — Find comparable properties (comps), analyze top neighborhoods, and get detailed neighborhood overviews.
- **Ownership & Sales** — Access ownership information, contact indicators, and historical sales data for specific properties.
- **Short-term Rental Data** — Retrieve Airbnb listings and short-term rental performance data to optimize your portfolio.

### How it works

1. Subscribe to this server
2. Enter your Mashvisor API Key
3. Start analyzing real estate markets from Claude, Cursor, or any MCP-compatible client

No more manual spreadsheet updates or jumping between tabs to find property owners. Your AI acts as a dedicated real estate analyst.

### Who is this for?

- **Real Estate Investors** — instantly retrieve investment performance, rental rates, and property comps to make data-driven decisions
- **Property Managers** — check market rental rates and neighborhood trends straight from your workflow
- **Real Estate Agents** — fetch ownership info and historical sales data to prepare for client meetings faster


## Available Tools (16)
- **get_airbnb_listings**: Get Airbnb performance metrics
- **get_city_investment_performance**: Get city investment performance
- **get_full_property_profile**: Get full property profile
- **get_historical_sales**: Get historical sales for a property
- **get_ownership_info**: Get ownership information
- **get_property_comps**: Find comparable properties (nearby)
- **get_property_details**: Get basic attributes for a specific property
- **get_historical_performance**: Get 36 months of historical STR performance
- **list_cities**: List cities in a specific state
- **get_marketplace_listings**: Search marketplace listings
- **get_neighborhood_overview**: Get neighborhood overview (bar)
- **get_rental_rates**: Get long-term rental rates
- **rento_calculator_lookup**: Rento-Calculator Lookup (Airbnb metrics)
- **search_properties**: Programmatic property search
- **get_top_neighborhoods**: List top neighborhoods
- **validate_city**: Validate a city name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mashvisor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for properties in Miami, FL with at least 3 beds and a price under $600,000."

**🤖 AI Agent:**
> I've found several properties in Miami matching your criteria. For example, a 3-bed property at [Address] is listed for $585,000. Would you like the full property profile for any of these?

---

**👤 You:**
> "Get the full property profile and historical sales for property ID 123456."

**🤖 AI Agent:**
> Fetching data for ID 123456... The profile includes a Mashvisor AVM of $450,000. Historical sales show it was last sold in 2018 for $310,000. It also has a tax history of $4,200 annually.

---

**👤 You:**
> "What are the top neighborhoods for investment in Orlando, FL?"

**🤖 AI Agent:**
> Analyzing Orlando market... The top neighborhoods based on investment performance are 'Downtown' (Cash on Cash: 5.2%) and 'Lake Nona' (Cash on Cash: 4.8%). Would you like a detailed overview of 'Downtown'?


## ❓ FAQ

**Q: Can I find comparable properties for a specific address to estimate its value?**
Yes! Use the `get_property_comps` tool by providing the property address or ID. The agent will return a list of nearby properties with similar characteristics to help you perform a comparative market analysis.

**Q: How do I check the investment performance of a specific city?**
You can use the `get_city_investment_performance` tool. Simply provide the state and city name, and the agent will retrieve key metrics like cash on return, cap rate, and rental income for that market.

**Q: Is it possible to get ownership information and contact details for a property?**
Yes, the `get_ownership_info` tool retrieves owner contact information and residency indicators for a specific property ID or address, allowing you to identify potential leads or current owners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mashvisor-alternative](https://vinkius.com/mcp/mashvisor-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mashvisor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mashvisor-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mashvisor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mashvisor-alternative": {
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
