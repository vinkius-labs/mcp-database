# SimplyRETS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplyrets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access real-time MLS real estate listings, agent data, and property analytics directly through your AI agent.

## Description
Connect your **SimplyRETS** account to any AI agent to query live MLS data, explore property metadata, and analyze real estate markets through natural language.

### What you can do

- **Property Search** — List and filter properties by location, price, or specific MLS identifiers using `list_properties`.
- **Deep Property Insights** — Fetch full details for a specific listing including features and school data with `get_property`.
- **Market Metadata** — Retrieve available cities, statuses, and property types within your feed using `get_property_metadata`.
- **Open Houses & Agents** — Access scheduled open house information and agent contact details via `list_open_houses` and `list_agents`.
- **Analytics** — Get data-driven insights and performance metrics for property listings with `get_property_analytics`.

### How it works

1. Subscribe to this server
2. Enter your SimplyRETS API Key and API Secret
3. Start querying real estate data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Agents** — quickly find property details and open house schedules without manual database searches.
- **Data Analysts** — extract market metadata and property analytics directly into your research workflow.
- **Developers** — test and query MLS data feeds through a conversational interface while building real estate apps.


## Available Tools (6)
- **list_agents**: List agent information
- **get_property**: Get details for a specific property listing
- **list_open_houses**: List open house information
- **list_properties**: List or search property listings
- **get_property_analytics**: Get analytics data for properties
- **get_property_metadata**: Get metadata about properties in a feed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimplyRETS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for active property listings in Houston with a limit of 5."

**🤖 AI Agent:**
> I found 5 active listings in Houston. One notable property is at 12402 Dakar (MLS: 123456) listed for $450,000. Would you like more details on any of these?

---

**👤 You:**
> "Show me all upcoming open houses from the MLS feed."

**🤖 AI Agent:**
> Retrieving open house data... I found 3 upcoming events. The next one is scheduled for 742 Evergreen Terrace this Sunday from 1 PM to 4 PM.

---

**👤 You:**
> "Get analytics for property MLS ID 123456."

**🤖 AI Agent:**
> Fetching analytics for MLS 123456... This property has seen a 5% increase in viewings this week and is priced 2% below the neighborhood average.


## ❓ FAQ

**Q: Can I search for properties in a specific city or area?**
Yes. Use the `list_properties` tool with the `q` parameter to search for specific locations, or use `points` for a geospatial polygon search.

**Q: How do I get the full details of a listing if I have the MLS ID?**
Simply provide the MLS ID to the `get_property` tool. It will return comprehensive metadata including price, features, and property history.

**Q: Can I see which agents are listed in the feed?**
Yes, the `list_agents` tool retrieves agent information directly from the MLS feed, allowing you to see contact details and affiliations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplyrets](https://vinkius.com/mcp/simplyrets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SimplyRETS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplyrets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SimplyRETS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplyrets": {
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
