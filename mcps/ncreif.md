# NCREIF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncreif)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access institutional commercial real estate data via NCREIF — track property performance, indices, and fund returns directly from your AI agent.

## Description
Connect your **NCREIF** account to your AI agent and gain authoritative insights into the institutional commercial real estate market through natural conversation.

### What you can do

- **Index Performance** — List and retrieve historical data for NCREIF indices such as the NPI (Property Index) and ODCE (Fund Index).
- **Property Oversight** — List indexed properties and fetch detailed historical returns and performance metrics.
- **Market Analysis** — Access high-level real estate market data and aggregated performance by region or property type (Office, Retail, etc.).
- **Fund Tracking** — View all tracked real estate investment funds and their performance history.
- **Data Series Access** — Browse granular data series and categories for in-depth real estate research.
- **Deep Inspection** — Fetch complete metadata for specific indices, properties, or funds using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your NCREIF API Key
3. Start querying commercial real estate intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Real Estate Analysts** — quickly check index returns or property performance without opening the NCREIF portal.
- **Portfolio Managers** — monitor institutional market trends and benchmark fund performance directly from your chat.
- **Investment Researchers** — automate the retrieval of complex real estate data series for reporting and modeling.


## Available Tools
- **get_fund_performance**: Get specific fund performance
- **get_index_data**: Get specific index data
- **get_property_returns**: Get property-level returns
- **get_property_type_data**: g., Office, Retail, Industrial).

Get data by property type
- **get_region_data**: Get performance data by region
- **list_data_series**: List available data series
- **list_funds**: List real estate funds
- **list_indices**: g., NPI, ODCE).

List NCREIF performance indices
- **list_market_data**: List real estate market data
- **list_properties**: List indexed properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NCREIF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all commercial real estate indices available via NCREIF."

**🤖 AI Agent:**
> I've retrieved the available indices. You have access to several primary benchmarks including the NPI (Property Index), the ODCE (Fund Index), and various regional sub-indices. Would you like to see the historical performance data for the NPI?

---

**👤 You:**
> "Show me the performance data for the 'Office' property type."

**🤖 AI Agent:**
> Retrieving data for property type 'Office' (ID: type_off)... In the last quarter, the total return was 1.2%, with income return at 1.1% and appreciation at 0.1%. Shall I compare this with the 'Industrial' property type performance?

---

**👤 You:**
> "What is the recent performance history for the ODCE Fund Index?"

**🤖 AI Agent:**
> Fetching data for the ODCE Index... For the trailing 12 months, the ODCE index returned 5.4%. The current market value of assets tracked by this index is over $300 billion. Would you like a breakdown of returns by fund size?


## ❓ FAQ

**Q: How do I get an NCREIF API Key?**
NCREIF API access is typically provided to member organizations. You can find or request your API key through the NCREIF Member Portal or by contacting their data services team.

**Q: What is the difference between NPI and ODCE indices?**
The NPI (NCREIF Property Index) tracks the performance of individual institutional properties, while the ODCE (Open End Diversified Core Equity) tracks the performance of diversified real estate funds.

**Q: Can I filter data by property type?**
Yes! Use the `get_property_type_data` tool to retrieve performance metrics specifically for categories like Office, Industrial, Retail, or Apartment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncreif](https://vinkius.com/mcp/ncreif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NCREIF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ncreif` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NCREIF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncreif": {
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
