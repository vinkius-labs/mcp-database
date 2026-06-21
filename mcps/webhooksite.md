# Webhook.site MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webhooksite)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/webhooksite-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/webhooksite-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test and debug webhooks and HTTP requests. Create custom URLs, inspect incoming payloads, and automate responses via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webhook.site** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Webhook.site token with the alias 'stripe-test' and a default 201 status."

**🤖 AI Agent:**
> I've created your new webhook token. The URL is https://webhook.site/stripe-test (ID: 550e8400-e29b-41d4-a716-446655440000). It is configured to return a 201 Created status by default.

---

**👤 You:**
> "Show me the 5 most recent requests received by token 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> I found 5 requests. The latest one was a POST request from IP 192.168.1.1 containing a JSON payload with 'event': 'payment.succeeded'. Would you like to see the full headers for this request?

---

**👤 You:**
> "Delete all requests for token 550e8400-e29b-41d4-a716-446655440000 that are older than 7 days."

**🤖 AI Agent:**
> I have successfully deleted all requests received before 'now-7d' for the specified token. Your request history is now cleared of older entries.


## Installation & Usage

To install and use the **Webhook.site** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webhooksite](https://vinkius.com/mcp/webhooksite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
