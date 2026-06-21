# Swiftfox MCP Server

Generate product mockups and marketing visuals instantly with AI that places your designs on real-world backgrounds.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/swiftfox)

## Overview
**Category:** communication-messaging
**Tools Count:** 11

## Description
Connect your **Swiftfox** account to any AI agent and take full control of your member management, engagement strategy, and communication campaigns through natural conversation.

### What you can do

- **Member Management** — List, query, and update individual member profiles and custom data fields.
- **Interaction Tracking** — Log notes, calls, and meetings to maintain a complete history of member engagement.
- **Campaign Insights** — Monitor the performance of your communication campaigns and verify outreach success.
- **Event Monitoring** — List and query interactions to stay on top of your community activity.
- **Operational Status** — Fetch account metadata and check API connectivity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Swiftfox API Key (found in your account settings)
3. Start managing your CRM ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Member Success Managers** — quickly retrieve profile details and log interactions via simple AI commands.
- **Campaign Coordinators** — monitor communication results and verify member segments directly from the workspace.
- **Non-Profit Leaders** — maintain organized records of community engagement and donor interactions via the AI assistant.


## Available Tools
- **check_swiftfox_status**: Returns a status indicator and account metadata to confirm valid credentials and active connectivity.

Verify Swiftfox API connectivity
- **get_event_fields**: Useful for understanding the data schema before creating or filtering events.

Get custom field definitions for events
- **get_organization**: Get full details of a specific organization in Swiftfox
- **get_person**: Get full details of a specific person in Swiftfox
- **list_circles**: Optionally filter by a search term matching circle names.

List circles (groups/domains/units) in Swiftfox
- **list_events**: Events represent meetings, functions, or activities organized within the CRM.

List events in Swiftfox CRM
- **list_organizations**: Organizations represent companies, associations, or groups that people belong to. Optionally filter by search term.

List organizations in Swiftfox CRM
- **list_people**: Optionally filter by a search term that matches against names or other fields.

List people (members) in Swiftfox CRM
- **list_webhooks**: Webhooks notify external services when specific events occur (e.g., member created, subscription updated).

List configured webhooks in Swiftfox
- **get_me**: Use this to verify connectivity or obtain the current user context.

Get the authenticated Swiftfox user profile
- **list_person_subscriptions**: Subscriptions track membership plans, payment status, and renewal dates.

List subscriptions for a specific person


## Installation & Usage

To install and use the **Swiftfox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swiftfox](https://vinkius.com/mcp/swiftfox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
