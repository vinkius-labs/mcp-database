# U.S. Treasury Debt — National Debt & Interest Rates MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-treasury-debt-national-debt-interest-rates-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-treasury-debt-national-debt-interest-rates-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access real-time data on the U.S. National Debt (currently $34T+). Retrieve 'Debt to the Penny', monitor average interest rates on Treasury securities, and access results from Treasury auctions.

## Description
U.S. Treasury debt data.

### 3 Tools
- **National Debt** — Debt to the Penny ($34T+)
- **Interest Rates** — Average interest rates on U.S. debt
- **Treasury Auctions** — Auction results for Bills, Notes, and Bonds

### Zero Auth


## Available Tools
- **get_national_debt**: S. national debt (Total Public Debt Outstanding) updated daily by the Treasury Department. Breaks down into Debt Held by the Public (marketable securities) and Intragovernmental Holdings (trust funds like Social Security). As of 2026, the national debt exceeds $39 trillion.

Get the U.S. national debt to the penny — updated daily
- **get_debt_history**: Format: YYYY-MM-DD. Useful for tracking debt growth over specific periods — fiscal years, election cycles, presidencies, economic crises.

Get national debt for a specific date range
- **get_public_debt_breakdown**: Shows both Debt Held by the Public and Intragovernmental Holdings.

Get the Statement of Public Debt — breakdown by security type
- **get_avg_interest_rates**: These rates reflect the cost of borrowing for the federal government. Updated monthly.

Get average interest rates on U.S. Treasury securities
- **get_treasury_auctions**: The bid-to-cover ratio indicates investor demand — higher ratios = stronger demand for U.S. debt.

Get results of Treasury securities auctions — Bills, Notes, Bonds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Treasury Debt — National Debt & Interest Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the exact current U.S. National debt?"

**🤖 AI Agent:**
> 📊 **U.S. Treasury: Debt to the Penny**

The most recent data (2026-03-31):
- Total Public Debt Outstanding: $34,812,456,789.12
- Intragovernmental Holdings: $7,123,456,789.12
- Debt Held by the Public: $27,689,000,000.00

---

**👤 You:**
> "What is the average interest rate on Treasury Bills?"

**🤖 AI Agent:**
> 📊 **U.S. Treasury Average Interest Rates**

Average interest rates for March 2026:
- Treasury Bills: 5.12%
- Treasury Notes: 4.58%
- Treasury Bonds: 4.75%

---

**👤 You:**
> "Show me the result of the last Treasury auction"

**🤖 AI Agent:**
> 📊 **Treasury Auctions**

Recent 10-Year Treasury Note Auction (2026-03-15):
- Amount Accepted: $42,000,000,000
- High Yield: 4.25%
- Bid-to-Cover Ratio: 2.54


## Installation & Usage

To install and use the **U.S. Treasury Debt — National Debt & Interest Rates** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates](https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
