# EasySendy MCP Server

Send high-volume email campaigns through multiple delivery servers with list hygiene tools that protect your sender score.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/easysendy)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect your **EasySendy** account to any AI agent and take full control of your email marketing lists and subscriber engagement workflows through natural conversation.

### What you can do

- **Audience Orchestration** — Create and manage email subscriber lists programmatically, including retrieving detailed metadata and custom tags
- **Subscriber Lifecycle** — Programmatically add, update, or remove subscribers from lists and manage detailed profiles directly from your agent
- **Batch Intelligence** — Perform large-scale subscriber imports and batch operations to streamline your high-volume marketing campaigns
- **Engagement Control** — Programmatically unsubscribe users or manage opt-in types (single/double) to ensure high-fidelity list hygiene and compliance
- **Field Customization** — Retrieve and manage custom contact fields and tags to maintain a structured and personalized communication ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Public API Key** from your EasySendy dashboard (Profile > APIs)
3. Start managing your email marketing lists from Claude, Cursor, or any MCP client

No more manual subscriber management or complex CSV exports in the dashboard. Your AI acts as your dedicated email marketing and list coordinator.

### Who is this for?

- **Growth Marketers** — instantly retrieve list details and manage segments using natural language queries
- **Marketing Operations** — automate lead ingestion and track custom tags across multiple lists without leaving your workspace
- **Business Owners** — monitor audience growth and manage subscriber lifecycles through simple AI commands


## Available Tools
- **add_multiple_subscribers**: Input should be an array of subscriber objects.

Add multiple subscribers to a list
- **add_subscriber**: Requires the List UID and at least an EMAIL address.

Add a single subscriber to a list
- **create_list**: Create a new subscriber list
- **delete_list**: Delete a subscriber list
- **delete_subscriber**: Delete a subscriber from a list
- **get_list_fields**: Get custom fields/tags for a list
- **get_subscriber_details**: Get details for a specific subscriber
- **list_all_lists**: List all subscriber lists
- **unsubscribe_user**: Unsubscribe a user from a list
- **update_list**: Update an existing subscriber list
- **update_subscriber**: Update an existing subscriber


## Installation & Usage

To install and use the **EasySendy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easysendy](https://vinkius.com/mcp/easysendy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
