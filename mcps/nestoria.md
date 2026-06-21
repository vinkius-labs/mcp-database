# Nestoria MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nestoria)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Search real estate listings globally — find properties to buy or rent across multiple countries with advanced filters.

## Description
Connect to **Nestoria**, the leading property search engine, and find your next home or investment through natural conversation. This server allows any AI agent to query thousands of real estate listings across the UK, Spain, France, Germany, Italy, Brazil, and Australia.

### What you can do

- **Global Property Search** — Search for listings in major markets using city names or specific coordinates.
- **Advanced Filtering** — Narrow down results by price range, number of bedrooms, and property types (houses, flats, etc.).
- **Buy vs. Rent** — Toggle between listings for sale or properties available for long-term rental.
- **Smart Sorting** — Order results by relevance, price (high/low), bedroom count, or the newest listings on the market.
- **Keyword Discovery** — Use specific terms like 'garden', 'pool', or 'renovated' to find properties that match your lifestyle.

### How it works

1. Subscribe to this server
2. (Optional) Provide a User Agent string for API identification
3. Start searching for properties directly from Claude, Cursor, or any MCP client

Stop jumping between dozens of real estate portals. Your AI agent can now aggregate and filter the best deals for you.

### Who is this for?

- **Home Buyers & Renters** — quickly find properties that meet specific criteria without manual searching
- **Real Estate Investors** — monitor market trends and new listings in specific regions
- **Relocation Specialists** — help clients find housing in new countries using localized search data


## Available Tools
- **search_listings**: Search for real estate listings on Nestoria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nestoria** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for houses to buy in London with at least 3 bedrooms."

**🤖 AI Agent:**
> I've found several houses in London with 3+ bedrooms. For example, a Victorian terrace in Fulham for £1,250,000 and a modern house in Greenwich. Would you like to see more details on these?

---

**👤 You:**
> "Find apartments for rent in Madrid between 1000 and 2000 euros."

**🤖 AI Agent:**
> Searching Nestoria Spain... I found 12 apartments in Madrid within your budget. Most are located in the Centro and Chamberí districts. Should I list them by price or newest first?

---

**👤 You:**
> "Look for properties in Paris with the keyword 'garden'."

**🤖 AI Agent:**
> I've filtered listings in Paris for 'garden'. I found a beautiful ground-floor flat in the 16th arrondissement and a house in Montmartre with a private courtyard. Would you like the full descriptions?


## ❓ FAQ

**Q: Can I search for properties using specific coordinates instead of a city name?**
Yes! Use the `search_listings` tool and provide the `centre_point` parameter with latitude and longitude separated by a comma (e.g., '51.50,-0.12').

**Q: How do I filter results by price and property type?**
You can use the `price_min`, `price_max`, and `property_type` (e.g., 'house' or 'flat') parameters within the `search_listings` tool to narrow down your search results.

**Q: Is it possible to see the newest listings first?**
Absolutely. Set the `sort` parameter to 'newest' when calling the `search_listings` tool to get the most recent entries at the top of your results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nestoria](https://vinkius.com/mcp/nestoria)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nestoria** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nestoria` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nestoria** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nestoria": {
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
