# Little Green Light MCP Server

Manage donor constituents, gifts, and appeals via the Little Green Light REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/little-green-light)

## Overview
**Category:** customer-relationship-management
**Tools Count:** 9

## Description
Connect your **Little Green Light** account to any AI agent to automate your donor management and fundraising workflows. This MCP server enables your agent to manage constituent profiles, record new gifts, and query fundraising appeals directly from natural language interfaces.

### What you can do

- **Constituent Oversight** — List and retrieve detailed profiles for all registered donors and organizations in your database
- **Gift Recording** — Programmatically record new donations, pledges, and recurring gifts with associated amounts and dates
- **Fundraising Audit** — Query active appeals, campaigns, and funds to monitor your fundraising efforts and allocations
- **Onboarding Automation** — Create new donor records and update existing contact information seamlessly
- **Database Discovery** — List all available organizational funds and campaign structures to map your financial logic

### How it works

1. Subscribe to this server
2. Enter your Little Green Light API Key (Bearer Token)
3. Start managing your donor relationships from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development Directors** — Monitor gift pipelines and donor engagement via simple natural language commands
- **Nonprofit Administrators** — Quickly update donor records and record donations without leaving your productivity tools
- **Philanthropy Tech Teams** — Integrate donor management logic and gift tracking into your custom internal dashboards


## Available Tools
- **list_fundraising_appeals**: List active fundraising appeals
- **list_fundraising_campaigns**: List fundraising campaigns
- **list_donor_constituents**: List donor constituents
- **create_new_donor**: Requires first_name, last_name, or org_name.

Create a new donor constituent
- **record_new_donation**: Requires constituent_id, amount, and gift_date.

Record a new donation gift
- **list_organizational_funds**: List available organizational funds
- **get_donor_details**: Get details for a specific constituent
- **get_gift_details**: Get details for a specific gift
- **list_donation_gifts**: List recorded gifts and donations


## Installation & Usage

To install and use the **Little Green Light** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/little-green-light](https://vinkius.com/mcp/little-green-light)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
