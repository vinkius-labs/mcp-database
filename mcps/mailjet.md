# Mailjet MCP Server

Send transactional emails and manage marketing campaigns via the Mailjet REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailjet)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **Mailjet** account to any AI agent to automate your transactional messaging and email marketing workflows. This MCP server enables your agent to send emails using the v3.1 Send API, manage subscriber lists, and track campaign performance directly from natural language interfaces.

### What you can do

- **Transactional Delivery** — Send single or batch emails with full support for HTML, attachments, and variables
- **Audience Management** — List all contacts, create new subscriber records, and manage contact lists (address books)
- **Subscription Control** — Add or remove contacts from specific lists and manage opt-in statuses programmatically
- **Campaign Tracking** — List historical campaigns and retrieve real-time performance statistics (opens, clicks, bounces)
- **Metadata Oversight** — Fetch detailed configuration and status for any campaign or subscriber collection

### How it works

1. Subscribe to this server
2. Enter your Mailjet API Public Key and Secret Key
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **Developers** — Quickly test email delivery and verify list logic directly from your IDE
- **Operations Teams** — Automate the synchronization of contact data and audit delivery performance effortlessly


## Available Tools
- **add_contact_to_list**: Requires list ID and contact ID/Email.

Subscribe a contact to a specific list
- **get_campaign_performance**: Get performance statistics for a campaign
- **create_new_contact**: Requires at least an Email address.

Add a new contact to the database
- **get_campaign_details**: Get details for a specific campaign
- **list_marketing_campaigns**: List all campaigns
- **list_subscriber_lists**: List all contact lists
- **list_all_contacts**: List all contacts in the Mailjet account
- **send_transactional_email**: Requires a JSON body matching Mailjet v3.1 Send API structure.

Send an email using Mailjet Send API v3.1


## Installation & Usage

To install and use the **Mailjet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailjet](https://vinkius.com/mcp/mailjet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
