# OneSignal MCP Server

Automate push notifications via OneSignal — send messages, manage segments, and track delivery stats directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/onesignal)

## Overview
**Category:** growth-engine
**Tools Count:** 10

## Description
Connect your **OneSignal** account to any AI agent and take full control of your customer engagement workflows through natural conversation.

### What you can do

- **Notifications Management** — Send, schedule, and cancel push notifications across mobile and web platforms.
- **Audience Targeting** — Target specific segments or individual player IDs to ensure the right message reaches the right user.
- **Delivery Analytics** — Fetch detailed reports and metrics for any notification to understand your engagement levels.
- **Device Management** — List, inspect, and manage registered devices (players) within your OneSignal applications.
- **App Overview** — List all your OneSignal apps and configurations to maintain a bird's-eye view of your notification infrastructure.

### How it works

1. Subscribe to this server
2. Enter your OneSignal REST API Key and App ID
3. (Optional) Provide your User Auth Key for account-level operations
4. Start engaging your users directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — instantly send campaign alerts or schedule upcoming announcements without touching the dashboard.
- **Support Teams** — check if a specific user received a notification by inspecting their player ID metadata.
- **Developers** — test notification payloads and verify device registrations directly from your development environment.


## Available Tools
- **cancel_notification**: Cancel a scheduled notification
- **create_notification**: Send a OneSignal notification
- **delete_player**: Delete a registered device
- **get_app**: Requires User Auth Key.

Get details for a specific OneSignal app
- **get_notification**: Get specific notification status
- **get_outcomes**: Get outcome data for the app
- **get_player**: Get specific player details
- **list_apps**: Requires User Auth Key.

List all OneSignal apps
- **list_notifications**: List notifications sent for the app
- **list_players**: List registered devices (players)


## Installation & Usage

To install and use the **OneSignal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesignal](https://vinkius.com/mcp/onesignal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
