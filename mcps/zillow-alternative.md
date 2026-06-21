# Zillow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zillow-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access real estate data, Zestimates, and property details directly from Zillow — search addresses, get valuations, and analyze market trends.

## Description
Connect your **Zillow** API access to any AI agent to retrieve comprehensive real estate data and property valuations through natural conversation.

### What you can do

- **Property Search** — Find specific properties using addresses and retrieve their unique Zillow Property IDs (ZPID) and basic Zestimates.
- **Deep Property Insights** — Access rich data including lot size, year built, bedroom/bathroom counts, and square footage for any target address.
- **Valuation & Zestimates** — Get the most recent Zestimate, valuation ranges, and rankings for millions of homes.
- **Market Comparisons** — Retrieve lists of comparable recent sales (comps) with detailed property data to understand local market value.
- **Visual Trends** — Generate URLs for historical Zestimate charts to visualize property value changes over 1, 5, or 10 years.
- **Demographics & Regions** — Fetch market affordability, real estate metrics, and demographic data for specific cities or neighborhoods.

### How it works

1. Subscribe to this server
2. Enter your Zillow Web Services ID (ZWSID)
3. Start querying real estate data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Investors** — quickly analyze potential deals, check comps, and view historical value trends without manual searching.
- **Home Buyers & Sellers** — get instant Zestimates and detailed property facts to make informed decisions.
- **Data Analysts** — retrieve regional demographics and market metrics directly into your workflow.


## Available Tools
- **get_chart**: Generates a URL for an image file displaying historical Zestimates
- **get_comps**: Returns a list of comparable recent sales
- **get_deep_comps**: ) for both the principal and comparable properties.

Returns rich property data for comparable properties
- **get_deep_search_results**: ) in addition to standard search results.

Finds a property and returns rich property data
- **get_demographics**: Returns demographic data for a specified region
- **get_monthly_payments**: Returns estimated monthly payments
- **get_rate_summary**: Returns current mortgage rates
- **get_region_chart**: Generates a URL for an image file displaying historical Zestimates for a region
- **get_region_children**: g., neighborhoods within a city) for a specified region.

Returns a list of subregions for a specified region
- **get_search_results**: Finds a property for a specified address
- **get_updated_property_details**: Returns home facts edited by the owner or agent
- **get_zestimate**: Returns the most recent Zestimate for a ZPID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zillow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the ZPID and Zestimate for 2150 N 107th St, Seattle, WA 98133."

**🤖 AI Agent:**
> I've located the property. The Zillow Property ID (ZPID) is 48749425. The current Zestimate is $845,000 with a valuation range between $802,000 and $887,000.

---

**👤 You:**
> "Show me 5 comparable sales for ZPID 48749425."

**🤖 AI Agent:**
> I've found 5 comparable sales near that property. Prices range from $820,000 to $865,000. Would you like the deep property details for these comps?

---

**👤 You:**
> "Generate a 5-year historical Zestimate chart for ZPID 48749425."

**🤖 AI Agent:**
> I've generated the chart URL for you. You can view the 5-year historical trend for this property here: [Chart URL]. It shows a steady 12% increase over the last period.


## ❓ FAQ

**Q: How can I get the estimated value of a home using its Zillow ID?**
Use the `get_zestimate` tool with the property's ZPID. It will return the current Zestimate, the valuation range, and its percentile ranking in the area.

**Q: Can I see detailed facts like square footage and year built for a specific address?**
Yes! The `get_deep_search_results` tool allows you to provide an address and city/state/zip to retrieve rich property data including beds, baths, lot size, and year built.

**Q: Is it possible to find demographic information for a specific neighborhood?**
Absolutely. Use the `get_demographics` tool and specify the neighborhood, city, or zip code to get market affordability and demographic metrics for that region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zillow-alternative](https://vinkius.com/mcp/zillow-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zillow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zillow-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zillow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zillow-alternative": {
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
