# Chatham Financial MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatham-financial)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chatham-financial-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chatham-financial-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage financial risk and valuations via Chatham Financial — track trades, monitor debt, and access market data directly from any AI agent.

## Description
Connect your **Chatham Financial (ChathamDirect)** account to any AI agent and take full control of your financial risk management and valuations through natural conversation. Streamline how you manage debt and derivatives.

### What you can do

- **Transaction Oversight** — List and retrieve details for derivative and debt transactions natively
- **Valuation Intelligence** — Access current and historical mark-to-market valuations flawlessly
- **Payment Tracking** — Monitor payment schedules and history for all financial instruments securely
- **Market Data Access** — Retrieve benchmark rates (SOFR, EURIBOR) and forward curves flawlessly
- **Hedge Accounting** — Access hedge accounting details and effectiveness test results flawlessly
- **Entity Management** — List all legal entities and portfolios configured in your account directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chatham API Key and Client ID (obtained from your relationship manager)
3. Start managing your financial risk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Treasury Managers** — monitor hedge performance and review trade valuations using natural language
- **Financial Controllers** — audit accounting entries and payment schedules without opening the complex dashboard
- **Risk Officers** — quickly verify market rates and hedge effectiveness results straight from their chat interface
- **Investment Analysts** — verify portfolio summaries and legal entity data for reporting


## Available Tools
- **get_trade_accounting**: Get hedge accounting details for a transaction
- **get_hedge_effectiveness**: Retrieve hedge effectiveness test results
- **get_chatham_market_data**: Retrieve benchmark rates and forward curves
- **get_trade_valuations**: Get current and historical valuations for a trade
- **list_chatham_entities**: List legal entities configured in the account
- **list_trade_payments**: List payment schedules and history for a transaction
- **list_chatham_portfolios**: List all managed portfolios
- **list_chatham_transactions**: List financial transactions and trades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chatham Financial** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active trades in my Chatham account."

**🤖 AI Agent:**
> Retrieving your active transactions... I found 12 instruments including 5 Interest Rate Swaps, 3 FX Forwards, and 4 Debt instruments. Which one would you like to see valuations for?

---

**👤 You:**
> "What is the latest valuation for trade ID 'T-98765'?"

**🤖 AI Agent:**
> Checking valuation for T-98765... The current mark-to-market value is +$45,230.50 as of yesterday's close. This is a 2.1% increase from the previous valuation.

---

**👤 You:**
> "Show me the forward curve for 3-month SOFR."

**🤖 AI Agent:**
> Retrieving SOFR 3M forward curve... The market expects rates to stay around 5.3% for the next 6 months, followed by a gradual decrease to 4.8% by mid-2025.


## Installation & Usage

To install and use the **Chatham Financial** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatham-financial](https://vinkius.com/mcp/chatham-financial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
