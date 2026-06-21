# Listmonk MCP Server

Automate your newsletter and mailing list management with Listmonk — manage subscribers, organize lists, and track campaigns directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/listmonk)

## Overview
**Category:** marketing-automation
**Tools Count:** 28

## Description
Connect your **Listmonk** instance to any AI agent and take full control of your email marketing workflows through natural conversation.

### What you can do

- **Subscriber Management** — List, create, update, or delete subscribers using SQL-like queries for precise filtering via `list_subscribers` and `create_subscriber`.
- **List Organization** — Manage your mailing lists and public subscriptions to keep your audience segmented using `list_lists` and `create_list`.
- **Campaign Control** — Create, monitor, and update the status of your email campaigns from draft to sent with `create_campaign` and `update_campaign_status`.
- **Transactional Emails** — Send high-priority transactional messages instantly via the `send_transactional` tool.
- **Media & Templates** — Manage your asset library and email templates without leaving your chat interface using `list_templates` and `list_media`.

### How it works

1. Subscribe to this server
2. Enter your Listmonk URL and API Token
3. Start managing your newsletters from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — quickly segment audiences and check campaign performance without opening the dashboard.
- **Developers** — integrate transactional emails and manage subscribers directly from the terminal or IDE.
- **Content Creators** — organize newsletter lists and templates with ease through simple commands.


## Available Tools
- **create_campaign**: Create a new campaign
- **create_list**: Create a new list
- **create_public_subscription**: Create a public subscription
- **create_subscriber**: Create a new subscriber
- **create_template**: Create a template
- **delete_bounces**: Delete multiple bounce records
- **delete_campaign**: Delete a campaign
- **delete_list**: Delete a list
- **delete_media**: Delete a media file
- **delete_subscriber**: Delete a specific subscriber
- **delete_template**: Delete a template
- **get_campaign**: Retrieve a specific campaign
- **get_import_status**: Retrieve import status
- **get_subscriber**: Retrieve a specific subscriber
- **list_bounces**: Retrieve bounce records
- **list_campaigns**: Retrieve all campaigns
- **list_lists**: Retrieve all lists
- **list_media**: Get uploaded media files
- **list_public_lists**: Retrieve public lists
- **list_subscribers**: Supports pagination, list filtering, and SQL expression search.

Query and retrieve subscribers
- **list_templates**: Retrieve all templates
- **patch_subscriber**: Partially update a subscriber
- **send_transactional_message**: Send transactional messages to one or more subscribers using a template
- **stop_import**: Stop an ongoing import
- **update_campaign_status**: Change campaign status
- **update_list**: Update a list
- **update_subscriber**: Update a specific subscriber
- **update_template**: Update a template


## Installation & Usage

To install and use the **Listmonk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listmonk](https://vinkius.com/mcp/listmonk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
