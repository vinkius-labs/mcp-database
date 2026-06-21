# BEA (Bureau of Economic Analysis) MCP Server

Access official US economic statistics including GDP, personal income, and industry data directly from the Bureau of Economic Analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bea-bureau-of-economic-analysis)

## Overview
**Category:** data-analytics
**Tools Count:** 4

## Description
The **BEA (Bureau of Economic Analysis)** MCP server provides a direct bridge to one of the world's most comprehensive sources of economic data. Empower your AI agent to retrieve, analyze, and report on the health of the US economy with precision.

### What you can do

- **Dataset Discovery** — Browse all available economic datasets including NIPA (National Income and Product Accounts), Regional, and Industry data.
- **Parameter Exploration** — Identify the specific filters and variables required for any dataset to ensure accurate queries.
- **Valid Value Lookup** — Retrieve lists of valid codes for parameters like TableID or Frequency to avoid API errors.
- **Data Retrieval** — Fetch raw economic figures, growth rates, and historical statistics directly into your conversation or analysis tool.

### How it works

1. Subscribe to this server
2. Enter your BEA API Key
3. Start querying economic indicators from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Researchers** — Quickly pull historical GDP or income data without manual CSV downloads.
- **Financial Analysts** — Integrate macroeconomic trends into market analysis and forecasting models.
- **Data Scientists** — Automate the ingestion of government-verified economic signals for machine learning projects.


## Available Tools
- **get_dataset_list**: g., NIPA, Regional, GDPByIndustry).

List available BEA datasets
- **get_data**: Pass dataset-specific parameters as a JSON string.

Retrieve economic data from a BEA dataset
- **get_parameter_list**: List parameters for a specific BEA dataset
- **get_parameter_values**: List valid values for a BEA dataset parameter


## Installation & Usage

To install and use the **BEA (Bureau of Economic Analysis)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bea-bureau-of-economic-analysis](https://vinkius.com/mcp/bea-bureau-of-economic-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
