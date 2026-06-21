# Zendesk Sell MCP Server

Manage sales leads, contacts, and deals via the Zendesk Sell (Base CRM) API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zendesk-sell)

## Overview
**Category:** sales-automation
**Tools Count:** 11

## Description
Connect your **Zendesk Sell** (formerly Base CRM) account to any AI agent to automate your sales pipeline and customer management. This MCP server enables your agent to interact with leads, qualified contacts, and sales deals directly from natural language interfaces.

### What you can do

- **Lead Management** — List, retrieve, and create sales leads to capture potential customer interest
- **Contact Oversight** — Manage qualified people and organizations, and retrieve their complete metadata profiles
- **Deal Tracking** — Monitor sales opportunities, update their status, and manage the entire deal lifecycle
- **Pipeline Automation** — Create and update sales records directly from your conversation to keep your CRM accurate
- **CRM Cleanup** — Delete unnecessary leads, contacts, or deals via simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your Zendesk Sell Personal Access Token
3. Start managing your sales CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — Quickly update deal statuses and lead notes without logging into the dashboard
- **Sales Managers** — Monitor pipeline health and track team opportunities via natural language commands
- **Operations Teams** — Automate the creation of sales records and maintain database hygiene effortlessly


## Available Tools
- **list_sales_contacts**: List all sales contacts (qualified prospects)
- **create_sales_contact**: Requires a JSON body with contact details.

Create a new person or organization contact
- **create_sales_deal**: Requires deal name and contact_id.

Create a new sales opportunity (deal)
- **create_new_lead**: Requires last_name or organization_name.

Create a new sales lead
- **list_sales_deals**: List all sales deals (opportunities)
- **delete_sales_deal**: Remove a deal from the account
- **get_sales_contact_details**: Get details for a specific contact
- **get_deal_details**: Get details for a specific sales deal
- **get_lead_details**: Get details for a specific lead
- **list_sales_leads**: List all sales leads
- **update_existing_deal**: Update details for an existing deal


## Installation & Usage

To install and use the **Zendesk Sell** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zendesk-sell](https://vinkius.com/mcp/zendesk-sell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
