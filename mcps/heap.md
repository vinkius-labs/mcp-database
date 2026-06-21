# Heap MCP Server

Automate product analytics via Heap — track events, identify users, and manage segments directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/heap)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect your **Heap.io** analytics account to any AI agent and take full control of your product data and user identity management through natural conversation.

### What you can do

- **Event Tracking** — Send custom server-side events to Heap to capture granular user interactions.
- **User Identification** — Associate anonymous sessions with specific identities and set custom profile properties.
- **Segment Management** — List all segments defined in your project to understand your user cohorts.
- **Event Definitions** — Access your custom event definitions to stay aligned with your analytics schema.
- **Bulk Operations** — Track multiple events or update several user profiles in a single high-throughput request.
- **GDPR Compliance** — Permanently delete user data directly from the chat interface when requested.
- **Query Profiles** — Filter and retrieve user profiles based on specific behavior or attributes.

### How it works

1. Subscribe to this server
2. Enter your Heap App ID and API Key
3. Start managing your product analytics from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex analytics dashboards for simple data updates. Your AI assistant acts as a dedicated Data Analyst or Growth Engineer.

### Who is this for?

- **Product Managers** — instantly check segment sizes and verify event definitions during planning.
- **Growth Engineers** — automate server-side event tracking and user property updates.
- **Data Privacy Officers** — streamline the execution of GDPR data deletion requests.


## Available Tools
- **add_account_properties**: Add or update properties for an account (group of users)
- **add_user_properties**: Add or update custom properties for a user profile
- **bulk_add_user_properties**: Update properties for multiple users in a single request
- **bulk_track_events**: Track multiple events concurrently for high-throughput
- **delete_user_data**: Permanently delete a user and all their associated data (GDPR)
- **get_api_usage**: Check current API usage and project status
- **get_my_profile**: Get information about the authenticated API key
- **identify_user**: Associate an anonymous session with a specific user identity
- **get_event_definitions**: List all custom event definitions in Heap
- **get_segments**: List all segments defined in your Heap project
- **query_user_profiles**: Query and filter user profiles based on criteria
- **track_event**: Properties should be a JSON string.

Track a server-side event for a user in Heap


## Installation & Usage

To install and use the **Heap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heap](https://vinkius.com/mcp/heap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
