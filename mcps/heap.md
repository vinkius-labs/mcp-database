# Heap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/heap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/heap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Automate product analytics via Heap — track events, identify users, and manage segments directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track event 'Checkout Started' for user 'user_992' with properties {'value': 49.99}."

**🤖 AI Agent:**
> Event tracked! I've successfully sent the 'Checkout Started' event for user_992 to Heap. Would you like to check the current properties for this user profile?

---

**👤 You:**
> "List all active segments in the project."

**🤖 AI Agent:**
> I've retrieved your segments. You have 5 active cohorts, including 'Power Users', 'Churn Risks', 'Trial Users', and 'New Signups'. Which segment would you like to query for user details?

---

**👤 You:**
> "Identify user 'anon_552' as 'john.doe@example.com'."

**🤖 AI Agent:**
> User identified! I've linked the anonymous session 'anon_552' to the identity 'john.doe@example.com' in Heap. Future events from this user will now be consolidated. Should I set any initial profile properties?


## Installation & Usage

To install and use the **Heap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heap](https://vinkius.com/mcp/heap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
