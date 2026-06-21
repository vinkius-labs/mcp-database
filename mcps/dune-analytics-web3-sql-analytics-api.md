# Dune Analytics (Web3 SQL Analytics API) MCP Server

Execute SQL queries on blockchain data via Dune Analytics — track executions, fetch results, and analyze Web3 metrics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api)

## Overview
**Category:** data-analytics
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Dune Analytics (Web3 SQL Analytics API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api](https://vinkius.com/mcp/dune-analytics-web3-sql-analytics-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
