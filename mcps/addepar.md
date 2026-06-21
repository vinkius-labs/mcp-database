# Addepar MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/addepar)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/addepar-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/addepar-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Investment management and reporting — manage portfolios, accounts, and financial performance via AI.

## Description
Connect your **Addepar** account to your AI agent to unlock enterprise-grade investment intelligence and reporting. From auditing portfolio performance to tracking granular transactions and managing complex ownership structures, your agent handles wealth management data through natural conversation.

### What you can do

- **Portfolio Intelligence** — Retrieve detailed performance and analytics for your clients and entity groups
- **Entity Management** — List and audit clients, accounts, and investment groups to maintain organizational clarity
- **Position Tracking** — View real-time holdings and ownership details across your entire investment landscape
- **Transaction Auditing** — Retrieve and analyze financial transaction logs to ensure accuracy and transparency
- **Metadata Insights** — Access deep technical metadata for any entity or account directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Addepar API Key, API Secret, and Firm ID
3. Start managing your wealth management data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Wealth Managers & Advisors** — quickly audit client portfolios and prepare for reviews using natural language
- **Investment Analysts** — retrieve granular position and transaction data for deeper analysis
- **Operations Teams** — manage entity metadata and verify data integrity across the platform
- **Family Offices** — track complex ownership structures and performance trends effortlessly


## Available Tools
- **list_entities**: List clients and accounts
- **get_entity_details**: Get details for an entity
- **get_portfolio_analytics**: Get portfolio performance data
- **get_position_details**: View portfolio holdings
- **list_transactions**: List financial transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Addepar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active client entities in my Addepar account."

**🤖 AI Agent:**
> I've retrieved the list of client entities. You have 15 active clients, including 'The Miller Family Office', 'East Coast Holdings', and 'Private Wealth Group'. Would you like to see the accounts for any of them?

---

**👤 You:**
> "Show me the performance for 'The Miller Family Office' for the last quarter."

**🤖 AI Agent:**
> I've analyzed the portfolio data. For the last quarter, 'The Miller Family Office' had a net return of 4.2% with a closing value of $12.5M. The top performing asset class was 'Global Equities'.

---

**👤 You:**
> "List the latest 10 transactions for account ID ACCT-123."

**🤖 AI Agent:**
> I've retrieved the latest 10 transactions for account ACCT-123. They include 5 buy trades, 3 dividend payments, and 2 cash transfers. Would you like the details for any specific transaction?


## Installation & Usage

To install and use the **Addepar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/addepar](https://vinkius.com/mcp/addepar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
