# Tyk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tyk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tyk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tyk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Tyk API Gateway and Dashboard — create keys, manage security policies, and list API definitions via natural language.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tyk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my API definitions sorted by name."

**🤖 AI Agent:**
> I've retrieved your API definitions. You have 3 active APIs: 'Auth-Service', 'Payment-Gateway', and 'User-Management'. Would you like to see the details for any of these?

---

**👤 You:**
> "Get the details for the security policy with ID 'pol-98765'."

**🤖 AI Agent:**
> Inspecting policy 'pol-98765'... This policy allows access to the 'Auth-Service' with a rate limit of 100 requests per minute and a quota of 10,000 requests per month.

---

**👤 You:**
> "Force a hot reload on the Tyk Gateway."

**🤖 AI Agent:**
> Triggering hot reload... The Tyk Gateway has successfully reloaded its configuration and all API definitions are now up to date.


## Installation & Usage

To install and use the **Tyk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tyk](https://vinkius.com/mcp/tyk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
