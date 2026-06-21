# Smartsheet MCP Server

Empower your AI to read Smartsheet rows, list workspaces, and manage your spreadsheets effortlessly from your code editor.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/smartsheet)

## Overview
**Category:** industry-titans
**Tools Count:** 6

## Description
Connect your **Smartsheet** account to any AI agent and empower your team to query project configurations, internal spreadsheets, and custom reports seamlessly. Interact with your organization's grids through natural language without ever switching tabs.

### What you can do

- **Project Navigation** — Easily map out your hierarchical structures calling `list_workspaces` and `list_folders` to find correct document locations
- **Sheet Deep-Dives** — Browse all your active spreadsheets using `list_sheets` and extract raw rows/columns instantly via `get_sheet_details`
- **Reporting Overviews** — Retrieve saved tabular aggregations automatically calling `list_reports` across all configured company sheets
- **Identity Profiling** — Test the connectivity and query authorized scopes by requesting the internal `get_current_user` tool

### How it works

1. Subscribe to this server
2. Enter your Personal Smartsheet Access Token
3. Start using Claude, Cursor, or any MCP-compatible client to query the state of your tabular data

Stop manually hunting down the ID of a specific project table just to wire up your Python scripts. Let your AI agent read the workspace layout automatically.

### Who is this for?

- **Project Managers** — rapidly audit how many tasks are active across cross-functional sheets or pull report overviews without exporting CSVs
- **Data Engineers** — query the actual sheet layout and row metadata directly from the code editor to build sturdy ETL scripts
- **Team Leaders** — have the bot read specific spreadsheets to generate weekly summary drafts completely autonomously


## Available Tools
- **list_sheets**: Lists all sheets available in Smartsheet
- **get_sheet_details**: Retrieves details for a specific sheet
- **list_workspaces**: Lists all workspaces in Smartsheet
- **list_folders**: Lists all folders
- **list_reports**: Lists all reports
- **get_current_user**: Retrieves information about the current Smartsheet user


## Installation & Usage

To install and use the **Smartsheet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartsheet](https://vinkius.com/mcp/smartsheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
