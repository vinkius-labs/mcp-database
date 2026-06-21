# Massive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/massive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access historical stock dividend data and distribution records directly from any AI agent.

## Description
Connect to **Massive** to retrieve comprehensive historical dividend data for thousands of tickers. Empower your AI agent to perform deep financial analysis and equity research through natural conversation.

### What you can do

- **Historical Dividends** — Fetch full records of cash distributions for any supported stock ticker from the Massive API.
- **Granular Filtering** — Filter results by ex-dividend date, frequency (annual, quarterly), or specific distribution types.
- **Distribution Types** — Identify recurring, special, supplemental, or irregular dividends to understand company payout patterns.
- **Data Analysis** — Sort and limit results (up to 5000 records) to build precise financial models or investment reports.

### How it works

1. Subscribe to this server
2. Enter your Massive API Key
3. Start querying financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly retrieve payout histories to calculate yields and dividend growth rates.
- **Investors** — check upcoming or historical ex-dividend dates to manage portfolio timing.
- **Developers** — integrate reliable financial distribution data into trading bots or research tools without complex scraping.


## Available Tools
- **list_dividends**: Retrieve historical cash dividends for a ticker


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Massive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List historical dividends for ticker 'AAPL'."

**🤖 AI Agent:**
> I've retrieved the dividend history for Apple Inc. (AAPL). Recent distributions include a recurring cash dividend of $0.25 with an ex-dividend date of 2024-05-10. Would you like to see the full list of historical payouts?

---

**👤 You:**
> "Show me special dividends for 'MSFT' sorted by date."

**🤖 AI Agent:**
> Searching for special distributions for Microsoft (MSFT)... I found a notable special dividend record from 2004-11-15 for $3.00. There are no other recent distributions flagged as 'special' in the database.

---

**👤 You:**
> "Find all dividends for 'KO' with a frequency of 4."

**🤖 AI Agent:**
> Querying quarterly dividends for Coca-Cola (KO)... I've found a consistent history of quarterly distributions (frequency: 4). The most recent was $0.48. Would you like to see the growth trend over the last 5 years?


## ❓ FAQ

**Q: Can I filter dividends by a specific date?**
Yes. You can use the `ex_dividend_date` parameter in the `list_dividends` tool to find distributions occurring on or after a specific YYYY-MM-DD date.

**Q: What types of dividend distributions can I identify?**
The `list_dividends` tool supports filtering by `distribution_type`, including 'recurring', 'special', 'supplemental', 'irregular', and 'unknown'.

**Q: How many dividend records can I retrieve at once?**
By default, the `list_dividends` tool returns 100 results, but you can increase the `limit` parameter up to a maximum of 5000 records per query.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/massive](https://vinkius.com/mcp/massive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Massive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `massive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Massive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "massive": {
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
