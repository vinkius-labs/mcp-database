# Massive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/massive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/massive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/massive-mcp)
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


## Installation & Usage

To install and use the **Massive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/massive](https://vinkius.com/mcp/massive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
