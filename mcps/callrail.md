# CallRail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callrail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/callrail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/callrail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage call tracking via CallRail — track calls, manage leads, and monitor marketing attribution directly from any AI agent.

## Description
Connect your **CallRail** account to any AI agent and orchestrate your call tracking, lead management, and marketing attribution workflows through natural conversation.

### What you can do

- **Call Oversight** — List all tracked phone calls and retrieve detailed metadata, including durations, tracking numbers, and statuses.
- **Lead Management** — Access leads generated via web forms and monitor their conversion journey directly from your workspace.
- **Company Coordination** — List and retrieve detailed profiles for all companies and clients managed within the account.
- **Tracker Oversight** — Monitor all active tracking numbers and their respective sources to ensure data accuracy.
- **User & Team Management** — Access your directory of users and agents to maintain visibility across your organization.
- **Alert Monitoring** — Retrieve and monitor active account alerts to stay on top of critical issues.

### How it works

1. Subscribe to this server
2. Enter your CallRail API Key and Account ID
3. Start managing your marketing attribution from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Analysts** — quickly check call volumes or source performance without manual dashboard exports.
- **Sales Managers** — monitor lead quality and form submissions straight from their workflow tools.
- **Agency Leads** — orchestrate client companies and tracking numbers using natural language.


## Available Tools
- **get_account_info**: Retrieve core account information
- **get_call_details**: Get details of a specific phone call
- **get_company_details**: Get details of a specific company
- **list_alerts**: List active account alerts
- **list_calls**: List all tracked phone calls
- **list_companies**: List all companies associated with the account
- **list_form_submissions**: List leads generated via web forms
- **list_tags**: List all lead and call tags
- **list_trackers**: List all tracking numbers and sources
- **list_users**: List all users in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallRail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my calls from today in CallRail."

**🤖 AI Agent:**
> I've retrieved your calls. You have 15 calls today, with an average duration of 3 minutes. The top source is 'Google Organic'.

---

**👤 You:**
> "Show the details for form submission with ID 99283."

**🤖 AI Agent:**
> Form submission 99283 was from 'John Doe' (john@example.com) on March 20th. The landing page was '/pricing'.

---

**👤 You:**
> "List all the companies in my CallRail account."

**🤖 AI Agent:**
> Retrieving companies... You have 3 active companies: 'Vinkius North', 'Global Solutions', and 'Tech Corp'. Which one would you like to see calls for?


## Installation & Usage

To install and use the **CallRail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callrail](https://vinkius.com/mcp/callrail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
