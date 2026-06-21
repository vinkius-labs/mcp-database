# Svix MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/svix)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/svix-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/svix-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your webhook infrastructure via Svix — orchestrate applications, configure endpoints, and monitor message delivery directly from any AI agent.

## Description
Connect your **Svix** account to any AI agent and take full control of your webhook lifecycle through natural conversation.

### What you can do

- **Application Management** — List, create, and update applications to group your endpoints and messages logically.
- **Endpoint Configuration** — Create and manage destination URLs, set event filters, and enable or disable specific endpoints for your apps.
- **Message Delivery** — Create and track messages, inspect payloads, and retrieve detailed delivery status for every event.
- **Debugging & Monitoring** — List message and endpoint attempts to identify failures and ensure your integrations are running smoothly.
- **Lifecycle Control** — Delete stale applications or endpoints and update configurations instantly without touching the dashboard.

### How it works

1. Subscribe to this server
2. Enter your Svix API Secret Key
3. Start managing your webhooks from Claude, Cursor, or any MCP-compatible client

No more manual debugging through logs. Your AI acts as a dedicated DevOps engineer for your event-driven architecture.

### Who is this for?

- **Backend Engineers** — quickly configure new webhook destinations and test event delivery without leaving the IDE.
- **DevOps Teams** — monitor delivery attempts and troubleshoot failing endpoints using natural language queries.
- **Product Integrations Leads** — manage customer-facing webhook applications and verify message flows in real-time.


## Available Tools
- **create_application**: Create a new Svix application
- **create_endpoint**: Create a new endpoint for a Svix application
- **create_message**: Send a new webhook message
- **delete_application**: Delete a Svix application
- **delete_endpoint**: Delete a Svix endpoint
- **get_application**: Get details of a specific Svix application
- **get_endpoint**: Get details of a specific Svix endpoint
- **get_message**: Get details of a specific Svix message
- **list_applications**: List Svix applications
- **list_endpoint_attempts**: List delivery attempts for a specific endpoint
- **list_endpoints**: List endpoints for a Svix application
- **list_message_attempts**: List delivery attempts for a specific message
- **list_messages**: List messages sent for a Svix application
- **update_application**: Update an existing Svix application
- **update_endpoint**: Update an existing Svix endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Svix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Svix applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 2 active apps: 'Main API' (ID: app_2X...) and 'Billing Service' (ID: app_9Y...). Which one would you like to inspect?

---

**👤 You:**
> "Create a new endpoint for app_2X... with URL https://webhook.site/test and subscribe to 'user.created' events."

**🤖 AI Agent:**
> Endpoint created successfully! The new endpoint ID is ep_3Z... and it is now configured to receive 'user.created' events at the specified URL.

---

**👤 You:**
> "Show me the details for message msg_4W..."

**🤖 AI Agent:**
> Fetching message details... Message msg_4W... was sent with event type 'invoice.paid'. It has been successfully delivered to 1 endpoint and is currently pending on another.


## Installation & Usage

To install and use the **Svix** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/svix](https://vinkius.com/mcp/svix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
