# Kindful MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kindful)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kindful-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kindful-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage nonprofit fundraising and donor relationships via Kindful — query contacts, track transactions, and monitor campaigns directly from your AI agent.

## Description
Connect your **Kindful** account to any AI agent to streamline your nonprofit operations and donor management through natural language.

### What you can do

- **Donor Management** — Query and filter contacts by groups, email status, or location using advanced keywords.
- **Transaction Tracking** — Monitor donations and financial records with precise date and campaign filters.
- **Campaign Insights** — List active fundraising campaigns to see goals, amounts raised, and overall progress.
- **Data Linking** — Connect Kindful records to external IDs to maintain synchronization with your other tools.
- **Organization Overview** — Retrieve metadata, custom fields, and group configurations specific to your nonprofit setup.

### How it works

1. Subscribe to this server
2. Enter your Kindful API Token and Subdomain
3. Start managing your fundraising data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development Directors** — instantly retrieve campaign statuses and donor lists without manual reporting
- **Data Managers** — sync external records and verify import stats directly through the agent
- **Nonprofit Admins** — quickly check organization details and custom field configurations


## Available Tools
- **create_import**: ).

Create an import job
- **get_campaigns**: Get campaigns
- **get_custom_fields**: Get custom fields
- **get_groups**: Get groups
- **get_import_stats**: Get import stats
- **get_import_status**: Get import job status
- **get_org_details**: Get organization details
- **link_contact**: Link a contact
- **link_transaction**: Link a transaction
- **query_contacts**: Query contacts in Kindful
- **query_transactions**: Query transactions in Kindful
- **verify_webhook**: Verify webhook event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kindful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active fundraising campaigns and show their current progress."

**🤖 AI Agent:**
> I've retrieved 3 active campaigns: 'Annual Gala' (Raised: $45,000 / Goal: $50,000), 'Clean Water Project' (Raised: $12,000 / Goal: $20,000), and 'Youth Education' (Raised: $5,500 / Goal: $10,000).

---

**👤 You:**
> "Search for Kindful contacts who have an email address and belong to group ID 789."

**🤖 AI Agent:**
> Searching... I found 12 contacts in Group 789 with valid email addresses. Would you like me to list their names and primary emails?

---

**👤 You:**
> "Show me all transactions recorded after 2024/01/01 for campaign ID 123."

**🤖 AI Agent:**
> I found 8 transactions for campaign 123 since January 1st, 2024, totaling $2,450. The largest single donation was $1,000 from donor ID 4567.


## Installation & Usage

To install and use the **Kindful** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kindful](https://vinkius.com/mcp/kindful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
