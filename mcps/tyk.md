# Tyk MCP Server

Manage your Tyk API Gateway and Dashboard — create keys, manage security policies, and list API definitions via natural language.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tyk)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **Tyk** instance to any AI agent to streamline your API management and gateway operations through conversation.

### What you can do

- **Key Management** — Create, retrieve, update, and delete API keys (Session Objects) directly in the Tyk Gateway.
- **Security Policies** — Define and manage security policies to control access rights and rate limits across your API ecosystem.
- **API Definitions** — List all active API definitions from your Dashboard and create new ones using the Tyk Classic format.
- **Gateway Control** — Trigger hot reloads to force the Gateway to refresh its configuration and apply changes instantly.
- **Granular Inspection** — Fetch detailed metadata for specific keys and policies to audit access and performance metrics.

### How it works

1. Subscribe to this server
2. Provide your Tyk URL and Gateway Secret (or Dashboard Token)
3. Start managing your API infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Automate gateway reloads and policy updates without leaving the terminal or chat interface.
- **Backend Developers** — Quickly generate API keys and check definition statuses during the development lifecycle.
- **Security Teams** — Audit existing policies and keys to ensure compliance with organizational access standards.


## Available Tools
- **create_api_definition**: Requires TYK_DASHBOARD_TOKEN.

Create a new API definition
- **create_key**: Requires TYK_GATEWAY_SECRET.

Create a new API key (Session Object)
- **create_org_key**: Requires TYK_ADMIN_SECRET.

Create an organization key
- **create_policy**: Requires TYK_GATEWAY_SECRET.

Create a new security policy
- **delete_key**: Requires TYK_GATEWAY_SECRET.

Delete an API key
- **delete_policy**: Requires TYK_GATEWAY_SECRET.

Delete a policy
- **get_key**: Requires TYK_GATEWAY_SECRET.

Get details for a specific API key
- **get_policy**: Requires TYK_GATEWAY_SECRET.

Get details of a single policy
- **hot_reload**: Requires TYK_GATEWAY_SECRET.

Force Gateway hot reload
- **list_apis**: Requires TYK_DASHBOARD_TOKEN.

List all API definitions
- **update_key**: Requires TYK_GATEWAY_SECRET.

Update an existing API key
- **update_policy**: Requires TYK_GATEWAY_SECRET.

Update an existing policy


## Installation & Usage

To install and use the **Tyk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tyk](https://vinkius.com/mcp/tyk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
