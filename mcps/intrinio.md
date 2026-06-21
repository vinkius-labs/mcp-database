# Intrinio MCP Server

Access real-time and historical financial market data via Intrinio API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/intrinio)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Empower your AI agents with Intrinio's comprehensive financial data. This MCP server allows you to retrieve real-time and historical stock prices, access financial statements, search for companies, and track earnings releases and IPO calendars directly through the Intrinio API. Ideal for financial analysis, portfolio monitoring, and market research.


## Available Tools
- **get_company**: g., "AAPL") or ID. Returns headquarters address, employee counts, and business descriptions. Useful for providing a profile overview of a company.

Retrieves details for a specific company
- **get_earnings_releases**: Essential for tracking reporting seasons and anticipating market volatility for specific tickers.

Lists upcoming and past earnings releases
- **get_financials**: Returns line items and values. Essential for fundamental financial analysis and performance vetting.

Retrieves financial statements for a company
- **get_ipo_calendar**: Useful for identifying new market entrants and investment opportunities.

Retrieves the IPO calendar
- **get_security**: Returns exchange info, security type, and identifiers. Use this to distinguish between different types of instruments traded under similar names.

Retrieves details for a specific security
- **get_stock_prices**: Use this to analyze market performance and price trends over time.

Retrieves historical stock prices for a security
- **list_companies**: Returns company names, tickers, and internal IDs. Use this to discover tickers before querying specific stock prices or financial statements.

Lists all companies covered by Intrinio
- **list_indices**: g., S&P 500, Dow Jones) tracked by Intrinio. Use this to identify index identifiers before querying index performance data.

Lists stock market indices
- **list_news**: Useful for monitoring market-moving events and recent announcements from public companies.

Lists latest financial news
- **search_companies**: Use this when the user provided a partial company name and you need to locate the correct ticker or ID.

Searches for companies by name or ticker


## Installation & Usage

To install and use the **Intrinio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intrinio](https://vinkius.com/mcp/intrinio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
