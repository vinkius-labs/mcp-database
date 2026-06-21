# ERS USDA (Economic Research) MCP Server

Access USDA Economic Research Service data, specifically the Agricultural Resource Management Survey (ARMS), covering farm finances and production.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ers-usda-economic-research)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect to the **USDA Economic Research Service (ERS)** and query the Agricultural Resource Management Survey (ARMS) directly. This server provides comprehensive access to the primary source of information on the financial condition, production practices, and resource use of America's farm businesses.

### What you can do

- **Survey Data Retrieval** — Fetch detailed financial and production data from U.S. farms using specific years, reports, or variables.
- **Geographic Analysis** — List all available ARMS States and retrieve metadata specific to regional agricultural economies.
- **Historical Trends** — Access all available survey years to perform longitudinal analysis of farm income and expenses.
- **Variable Metadata** — Inspect detailed definitions and metadata for variables used in the ARMS dataset to ensure accurate data interpretation.
- **Farm Classification** — Query specific farm types and categories (like farm typology or operator households) to segment your research.

### How it works

1. Subscribe to this server
2. Enter your ERS USDA API Key
3. Start querying agricultural economic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agricultural Economists** — quickly pull survey results for income statements and balance sheets without manual exports.
- **Data Analysts** — integrate official government agricultural metrics into broader economic models or reports.
- **Policy Researchers** — analyze farm household characteristics and production practices across different U.S. states.


## Available Tools
- **get_arms_categories**: List ARMS categories and subcategories
- **get_arms_farmtypes**: Get all ARMS Farm Types
- **get_arms_reports**: Get available ARMS reports and variables
- **get_arms_states**: Get all ARMS States and available metadata
- **get_arms_surveydata**: S. farms. Requires year AND at least one of report or variable.

Retrieve ARMS survey results
- **get_arms_variables**: Get detailed metadata for ARMS variables
- **get_arms_years**: Get all available ARMS years


## Installation & Usage

To install and use the **ERS USDA (Economic Research)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ers-usda-economic-research](https://vinkius.com/mcp/ers-usda-economic-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
