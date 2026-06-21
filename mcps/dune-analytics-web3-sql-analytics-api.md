# Dune Analytics (Web3 SQL Analytics API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dune-analytics-web3-sql-analytics-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dune-analytics-web3-sql-analytics-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Execute SQL queries on blockchain data via Dune Analytics — track executions, fetch results, and analyze Web3 metrics directly from your AI agent.

## Description
Connect your **Dune Analytics** account to any AI agent to query and analyze real-time blockchain data using SQL. Access comprehensive datasets across Ethereum, Solana, Polygon, and more through natural conversation.

### What you can do

- **Query Execution** — Trigger any existing Dune query ID with custom parameters to refresh on-chain data.
- **Status Tracking** — Monitor the lifecycle of your SQL executions from pending to completion using execution IDs.
- **Data Retrieval** — Fetch large result sets directly into your agent for immediate analysis, visualization, or reporting.
- **Execution Control** — Cancel long-running or unnecessary queries to optimize your API usage and credits.

### How it works

1. Subscribe to this server
2. Enter your Dune API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull the latest DeFi, NFT, or DAO metrics without leaving your workspace.
- **Web3 Developers** — verify on-chain states, protocol health, and contract interactions directly from your code editor.
- **Crypto Researchers** — automate the gathering of ecosystem growth data and market trends for reports.


## Available Tools
- **cancel_execution**: Interrupt an ongoing query execution
- **execute_query**: Returns an execution_id to track status.

Execute a specific Dune query ID with optional parameters
- **get_execution_results**: Use get_execution_status first to ensure it is completed.

Retrieve the data rows from a completed execution
- **get_execution_status**: g., QUERY_STATE_PENDING, QUERY_STATE_COMPLETED, QUERY_STATE_FAILED).

Check the current status of a query execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dune Analytics (Web3 SQL Analytics API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Execute Dune query ID 1234567 with parameters for the last 7 days."

**🤖 AI Agent:**
> I've started the execution for query 1234567. The execution ID is '01J8X...'. I will monitor the status for you.

---

**👤 You:**
> "Check the status of my Dune execution 01J8X9Z..."

**🤖 AI Agent:**
> The execution 01J8X9Z... is currently 'QUERY_STATE_COMPLETED'. Would you like me to fetch the results now?

---

**👤 You:**
> "Fetch the results for execution ID 01J8X9Z... and summarize the top 5 holders."

**🤖 AI Agent:**
> I've retrieved the data. Based on the results, the top 5 holders are: 1) 0xabc... with 500 ETH, 2) 0xdef... with 450 ETH...


## Installation & Usage

To install and use the **Dune Analytics (Web3 SQL Analytics API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api](https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
