# Courier MCP Server

Equip your AI agent to send multi-channel notifications and monitor delivery status through the Courier API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/courier)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Courier**, the smart notification infrastructure, directly into your AI workflow. Design, orchestrate, and send messages across email, SMS, push, and chat apps using natural language.

### What you can do

- **Send Notifications** — Trigger complex notification workflows to any recipient via the Send API.
- **Message Monitoring** — List sent messages and track their real-time delivery status (sent, delivered, opened).
- **Template Management** — Browse available notification templates and custom brands.
- **Audience & User Insights** — Manage subscription lists and retrieve user profiles.

### How it works

1. Connect the Courier integration to your AI assistant.
2. Authorize using your Courier Auth Token (found in Settings > API Keys).
3. Manage your global notification strategy through chat.

### Who is this for?

- **Product Managers** — Quickly verify if critical system notifications are being delivered.
- **Developers** — Audit message history and troubleshoot delivery issues via chat.
- **Customer Support** — Check user profiles and their recent notification history to provide better help.


## Available Tools
- **get_message_history**: Resolves event types (SENT, DELIVERED, etc.) and detailed provider logs.

Get the delivery history logs for a message
- **get_message_details**: Touches delivery logs, provider responses, and rendering metadata boundary.

Get details for a specific message by ID
- **get_user_profile**: Resolves contact details (email, phone) and channel-specific delivery preferences.

Get the profile data for a specific user
- **list_audiences**: Resolves audience IDs, names, and filter criteria used for segmentation.

List saved audiences for targeted notifications
- **list_brands**: Resolves brand names, colors, and logo settings used for white-labeling notifications.

List custom brands configured in Courier
- **list_subscription_lists**: Resolves list IDs, names, and subscriber counts.

List subscription lists for managing recipients
- **list_messages**: Resolves message IDs, recipient identifiers, status (SENT, DELIVERED, OPENED, CLICKED), and timestamps.

List sent messages and their current status
- **list_templates**: Resolves template names, IDs, and supported channels.

List available notification templates
- **list_users**: Resolves user IDs, roles, and account association details.

List users registered in the Courier workspace
- **send_notification**: Touches recipient profile, template engine, and multi-channel provider boundaries.

Send a notification to a recipient


## Installation & Usage

To install and use the **Courier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/courier](https://vinkius.com/mcp/courier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
