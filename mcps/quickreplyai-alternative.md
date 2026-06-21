# QuickReply.ai MCP Server

Automate WhatsApp marketing and customer engagement via QuickReply.ai — trigger journeys, send templates, and manage session messages directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/quickreplyai-alternative)

## Overview
**Category:** communication-messaging
**Tools Count:** 5

## Description
Connect **QuickReply.ai** to your AI agent and orchestrate your WhatsApp marketing and customer communication through natural conversation.

### What you can do

- **Automated Journeys** — Trigger personalized WhatsApp journeys using the `trigger_journey_event` tool with specific receiver IDs.
- **Template Messaging** — Send pre-approved WhatsApp templates with dynamic variables using `send_template` for official notifications.
- **Session Conversations** — Send free-form text and images within the 24-hour service window using `send_session_message`.
- **Drip Campaigns** — Schedule and trigger automated drip sequences for user nurturing with `trigger_drip_campaign`.
- **Performance Analytics** — Retrieve detailed message-level statistics and insights using `fetch_campaign_stats`.

### How it works

1. Subscribe to this server
2. Enter your QuickReply.ai Client ID and Secret Key
3. Start managing your WhatsApp outreach from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Launch campaigns and track performance without switching between multiple dashboards.
- **Customer Support Teams** — Respond to users with session messages and send automated updates via templates.
- **Sales & Growth Leads** — Automate lead nurturing journeys and follow-up sequences directly through AI orchestration.


## Available Tools
- **fetch_campaign_stats**: Note: This API will sunset in June 2026.

Fetch campaign messages stats
- **send_session_message**: Send a free-form session message
- **send_template**: Send a pre-approved WhatsApp template
- **trigger_drip_campaign**: Note: This API will sunset in June 2026.

Trigger a specific drip campaign for a user
- **trigger_journey_event**: This is the recommended way to trigger messages.

Trigger a journey via Webhook Data Source


## Installation & Usage

To install and use the **QuickReply.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickreplyai-alternative](https://vinkius.com/mcp/quickreplyai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
