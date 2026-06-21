# Mail Blaze MCP Server

Manage email marketing campaigns and subscriber lists via the Mail Blaze REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mail-blaze)

## Overview
**Category:** marketing-automation
**Tools Count:** 9

## Description
Connect your **Mail Blaze** account to any AI agent to automate your email marketing and audience management. This MCP server enables your agent to manage subscriber lists, create and send campaigns, and track subscriber updates directly from natural language interfaces.

### What you can do

- **Campaign Management** — List all email campaigns and retrieve detailed metadata and status information
- **Instant Sending** — Trigger the delivery of existing campaigns to your targeted lists instantly
- **List Oversight** — Manage subscriber lists and retrieve their unique identifiers for grouping
- **Subscriber Control** — Add, update, and remove subscribers from specific lists while managing custom fields
- **Draft Creation** — Initialize new campaign drafts directly from your conversation to streamline your marketing workflow

### How it works

1. Subscribe to this server
2. Enter your Mail Blaze API Public Key (X-MW-PUBLIC-KEY)
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Monitor campaign statuses and manage subscriber segments via simple natural language commands
- **Marketing Operations** — Quickly update contact information and trigger campaign sends without opening the dashboard
- **Developers** — Integrate email automation logic and subscriber management into your custom internal tools


## Available Tools
- **add_subscriber_to_list**: Requires a list UID and subscriber data.

Add a new subscriber to a list
- **list_email_campaigns**: List all email marketing campaigns
- **create_new_campaign**: Requires a JSON body with campaign details.

Create a new email marketing campaign
- **delete_list_subscriber**: Remove a subscriber from a list
- **get_campaign_details**: Get details for a specific campaign
- **list_list_subscribers**: List subscribers in a specific list
- **list_subscriber_lists**: List all subscriber lists
- **send_email_campaign**: Trigger the sending of a campaign
- **update_list_subscriber**: Update an existing subscriber


## Installation & Usage

To install and use the **Mail Blaze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mail-blaze](https://vinkius.com/mcp/mail-blaze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
