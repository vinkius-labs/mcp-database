# Rightmove MCP Server

Manage Rightmove property listings, track performance metrics, and retrieve branch leads directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rightmove)

## Overview
**Category:** real-estate
**Tools Count:** 4

## Description
Connect your **Rightmove** real-time data feed to any AI agent to streamline your estate agency operations. This server allows you to manage the entire lifecycle of a property listing and monitor its success without leaving your AI interface.

### What you can do

- **Listing Management** — Create new property listings or update existing ones with detailed address, price, and media information using the `send_property` tool.
- **Inventory Control** — Remove properties from the portal using specific reason codes like 'Sold' or 'Withdrawn' via `remove_property`.
- **Lead Retrieval** — Fetch email leads sent by potential buyers or tenants for specific branches over defined periods with `get_branch_emails`.
- **Performance Tracking** — Analyze how your listings are performing with data on search appearances and detail views using `get_property_performance`.

### How it works

1. Subscribe to this server
2. Provide your Rightmove Network ID, Certificate, and Private Key
3. Start managing your property portfolio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Estate Agents** — Update listings and check leads instantly during client meetings or on the go.
- **Data Analysts** — Pull performance metrics to generate reports on property engagement and market trends.
- **Operations Managers** — Automate the removal of sold properties and sync inventory across platforms efficiently.


## Available Tools
- **get_branch_emails**: Retrieve lead information (emails) for a specific branch
- **get_property_performance**: Retrieve performance statistics for a specific listing
- **remove_property**: Remove a property from the Rightmove website
- **send_property**: If the agent_ref already exists, the property is updated.

Add a new property or update an existing one on Rightmove


## Installation & Usage

To install and use the **Rightmove** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rightmove](https://vinkius.com/mcp/rightmove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
