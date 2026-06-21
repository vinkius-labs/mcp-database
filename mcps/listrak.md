# Listrak MCP Server

Manage email and SMS campaigns, contacts, and messaging via the Listrak REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/listrak)

## Overview
**Category:** marketing-automation
**Tools Count:** 7

## Description
Connect your **Listrak** account to any AI agent to automate your cross-channel marketing and transactional messaging. This MCP server enables your agent to manage email and SMS campaigns, interact with contact profiles, and trigger immediate broadcasts directly from natural language interfaces using OAuth 2.0.

### What you can do

- **Email Campaign Management** — List all active and historical email campaigns to monitor your marketing objectives
- **SMS Engagement** — List, create, and manage SMS contacts, and subscribe users to specific phone-based lists
- **Transactional Messaging** — Trigger pre-defined transactional emails instantly for order confirmations, alerts, or notifications
- **Instant Broadcasts** — Send immediate SMS broadcast messages to your audience using your configured sender codes
- **Contact Insights** — Retrieve detailed profile information for email contacts across your organizational lists
- **Database Maintenance** — Create new SMS profiles and manage cross-channel subscriptions effortlessly

### How it works

1. Subscribe to this server
2. Enter your Listrak Client ID and Client Secret
3. Start managing your cross-channel marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **CRM Managers** — Monitor campaign statuses and manage subscriber lists via simple natural language commands
- **Marketing Operations** — Quickly trigger transactional alerts and verify contact data without opening the portal
- **Growth Engineers** — Integrate email and SMS automation logic directly into your custom internal tools


## Available Tools
- **send_sms_broadcast**: Send an immediate SMS broadcast
- **create_sms_contact**: Add a new SMS contact
- **list_email_campaigns**: List all email campaigns
- **get_email_contact_details**: Get details for a specific email contact
- **list_sms_contacts**: List SMS contacts
- **send_transactional_email**: Requires messageId and recipient data.

Send a transactional email
- **subscribe_to_sms_list**: Subscribe a contact to an SMS list


## Installation & Usage

To install and use the **Listrak** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listrak](https://vinkius.com/mcp/listrak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
