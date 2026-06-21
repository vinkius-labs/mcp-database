# Webhook.site MCP Server

Test and debug webhooks and HTTP requests. Create custom URLs, inspect incoming payloads, and automate responses via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/webhooksite)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect **Webhook.site** to your AI agent to instantly create, manage, and inspect HTTP webhooks. Perfect for debugging integrations, testing callbacks, and automating API workflows through natural conversation.

### What you can do

- **Token Management** — Create new webhook URLs (tokens) with custom aliases, expiry times, and default response behaviors.
- **Request Inspection** — List and retrieve detailed metadata for all incoming HTTP requests, including headers, query parameters, and raw payloads.
- **Dynamic Responses** — Set custom HTTP status codes, headers, and body content for specific requests to simulate complex API behaviors.
- **Automated Actions** — List and execute configured actions on your tokens to automate your development pipeline.
- **Global Variables** — Manage environment-wide variables to maintain state across different webhook tests.

### How it works

1. Subscribe to this server
2. Enter your Webhook.site API Key
3. Start debugging webhooks directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — test webhooks without setting up local tunnels or public servers.
- **QA Engineers** — validate third-party callbacks and simulate various API response scenarios.
- **DevOps Teams** — monitor incoming alerts and automate response triggers via AI-driven actions.


## Available Tools
- **create_action**: Create a custom action for a token
- **create_global_variable**: Create a global variable
- **create_token**: Create a new Webhook.site token (URL)
- **delete_action**: Delete a custom action
- **delete_global_variable**: Delete a global variable
- **delete_requests**: Delete multiple requests for a token
- **delete_token**: Delete a token
- **execute_action**: Execute actions for a specific request
- **get_requests**: Get requests captured by a token
- **get_token**: Get details for a specific token
- **list_actions**: List custom actions for a token
- **list_global_variables**: List global variables
- **list_tokens**: List Webhook.site tokens
- **set_response**: Set dynamic response for a specific request
- **update_action**: Update a custom action
- **update_global_variable**: Update a global variable
- **update_token**: Update an existing token


## Installation & Usage

To install and use the **Webhook.site** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webhooksite](https://vinkius.com/mcp/webhooksite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
