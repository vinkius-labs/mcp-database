# Little Green Light MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/little-green-light)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/little-green-light-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/little-green-light-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage donor constituents, gifts, and appeals via the Little Green Light REST API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Little Green Light** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all constituents in my Little Green Light account."

**🤖 AI Agent:**
> I've retrieved your constituents. You have 15 registered profiles, including 'John Smith', 'Alice Doe', and 'The Acme Foundation'. Would you like to see details for any of them?

---

**👤 You:**
> "Record a new donation of $100.00 for constituent ID '12345' dated today."

**🤖 AI Agent:**
> Successfully recorded the gift of $100.00 for constituent 12345. The gift has been added to your records with today's date.

---

**👤 You:**
> "Show active fundraising appeals."

**🤖 AI Agent:**
> I found 3 active appeals: 'Winter Mailing 2024 (ID: 987)', 'Annual Gala (ID: 654)', and 'Building Fund (ID: 321)'.


## Installation & Usage

To install and use the **Little Green Light** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/little-green-light](https://vinkius.com/mcp/little-green-light)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
