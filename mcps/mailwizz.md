# MailWizz MCP Server

Manage email marketing campaigns and subscriber lists via the MailWizz REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailwizz)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **MailWizz** instance to any AI agent to automate your professional email marketing and audience management. This MCP server enables your agent to manage subscriber lists, control campaign lifecycles, and update subscriber data directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all email campaigns and retrieve detailed metadata and status information
- **Mailing Control** — Pause or unpause campaigns and manage their delivery lifecycle programmatically
- **Audience Management** — List all subscriber collections (lists) and retrieve their unique identifiers
- **Subscriber Administration** — Add, update, and remove subscribers from specific lists using their UIDs
- **Data Ingestion** — Sync subscriber information and manage custom fields across your email databases
- **Self-Hosted Support** — Works with any self-hosted MailWizz instance using your personal API keys

### How it works

1. Subscribe to this server
2. Enter your MailWizz API URL and Public Key
3. Start managing your marketing audience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **CRM Specialists** — Quickly update contact information and audit list health without leaving your productivity tools
- **Developers** — Integrate MailWizz's robust marketing logic into your custom internal tools


## Available Tools
- **add_subscriber_to_list**: Requires a list UID and subscriber data.

Add a new subscriber to a list
- **list_email_campaigns**: List all email marketing campaigns
- **delete_list_subscriber**: Remove a subscriber from a list
- **get_campaign_details**: Get details for a specific campaign
- **get_list_details**: Get details for a specific subscriber list
- **list_list_subscribers**: List subscribers in a specific list
- **list_subscriber_collections**: List all subscriber lists
- **pause_email_campaign**: Pause a running campaign
- **update_list_subscriber**: Update an existing subscriber


## Installation & Usage

To install and use the **MailWizz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailwizz](https://vinkius.com/mcp/mailwizz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
