# Patreon (Creator Subscriptions) MCP Server

Manage your Patreon creator account—list campaigns, track members, and monitor posts directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/patreon-creator-subscriptions)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Patreon** creator account to any AI agent to streamline your membership management and content workflow.

### What you can do

- **Campaign Overview** — List and fetch detailed information about your active Patreon campaigns using `list_campaigns` and `get_campaign`.
- **Member Management** — Retrieve lists of members and inspect individual member details with `list_campaign_members` and `get_member` to understand your audience.
- **Content Monitoring** — Access all posts associated with your campaigns via `list_campaign_posts` to stay on top of your content schedule.
- **Webhook Integration** — Create, list, and manage webhooks for real-time notifications on member activity and post updates using `create_webhook`, `list_webhooks`, and `delete_webhook`.
- **Identity Verification** — Quickly check your authenticated profile and associated permissions with `get_identity`.

### How it works

1. Subscribe to this server
2. Enter your Patreon Creator Access Token
3. Start managing your creator ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Get instant summaries of your membership base and post history without leaving your workflow.
- **Community Managers** — Track member growth and engagement metrics through natural language queries.
- **Developers** — Build and test webhook integrations for custom creator tools directly from the IDE.


## Available Tools
- **list_campaigns**: List campaigns owned by the user
- **create_webhook**: g., members:create, posts:publish).

Create a new webhook
- **delete_webhook**: Delete a webhook
- **get_campaign**: Get details for a specific campaign
- **get_member**: Get details for a specific member
- **get_identity**: Can include memberships and campaign data.

Get the authenticated user profile
- **list_campaign_members**: List members for a specific campaign
- **list_campaign_posts**: List all posts for a campaign
- **update_webhook**: Update an existing webhook
- **list_webhooks**: List webhooks created by your client


## Installation & Usage

To install and use the **Patreon (Creator Subscriptions)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/patreon-creator-subscriptions](https://vinkius.com/mcp/patreon-creator-subscriptions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
