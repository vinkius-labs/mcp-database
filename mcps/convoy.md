# Convoy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convoy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/convoy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/convoy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage webhooks with Convoy — create endpoints, broadcast events, and monitor delivery directly from your AI agent.

## Description
Connect **Convoy** to your AI agent to orchestrate and monitor your webhook infrastructure through natural conversation.

### What you can do

- **Endpoint Management** — Create, list, update, and delete destination endpoints for your webhooks.
- **Event Delivery** — Create specific events or broadcast them to all matching endpoints in your project.
- **Operational Control** — Pause or activate endpoints instantly to manage traffic flow and maintenance.
- **Project Monitoring** — Retrieve detailed metadata for specific endpoints to debug delivery issues.

### How it works

1. Subscribe to this server
2. Enter your Convoy API Key and Base URL
3. Start managing your webhook pipeline from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly toggle endpoint states and monitor delivery health.
- **Backend Developers** — trigger test events and manage webhook configurations without leaving the terminal or IDE.
- **SREs** — automate the response to webhook delivery failures by inspecting endpoint statuses.


## Available Tools
- **activate_endpoint**: Activate a paused endpoint
- **batch_retry_event_deliveries**: Batch retry event deliveries
- **broadcast_event**: Create a broadcast event
- **bulk_create_filters**: Bulk create filters for a subscription
- **bulk_onboard**: Bulk onboard endpoints and subscriptions
- **create_endpoint**: Create a new Convoy endpoint
- **create_event**: Create a new event
- **create_event_type**: Create an event type
- **create_filter**: Create a filter for a subscription
- **create_portal_link**: Create a portal link
- **create_source**: Create a source
- **create_subscription**: Create a subscription
- **delete_endpoint**: Delete an endpoint
- **dynamic_event**: Create a dynamic event
- **fanout_event**: Fan out an event
- **get_delivery_attempt**: Retrieve a specific delivery attempt
- **get_endpoint**: Retrieve a specific endpoint
- **import_event_types**: Import event types from OpenAPI
- **list_delivery_attempts**: List delivery attempts for an event delivery
- **list_endpoints**: List all endpoints in a project
- **list_event_deliveries**: List event deliveries
- **list_meta_events**: List meta events
- **list_subscriptions**: List subscriptions
- **pause_endpoint**: Pause an endpoint
- **retry_event_delivery**: Retry an event delivery
- **update_endpoint**: Update an existing endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convoy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all endpoints for project 'proj_123'."

**🤖 AI Agent:**
> I've retrieved the endpoints for project 'proj_123'. You have 3 active endpoints: 'Staging Webhook' (ID: end_001), 'Production Sync' (ID: end_002), and 'Analytics Collector' (ID: end_003).

---

**👤 You:**
> "Create a new endpoint named 'Production Webhook' at 'https://api.example.com/webhook' for project 'proj_123'."

**🤖 AI Agent:**
> The endpoint 'Production Webhook' has been successfully created in project 'proj_123' with ID 'end_999'. It is now ready to receive events.

---

**👤 You:**
> "Broadcast an event of type 'user.signup' with data '{"id": 1}' in project 'proj_123'."

**🤖 AI Agent:**
> Broadcasting the 'user.signup' event... The event has been dispatched to all matching endpoints in project 'proj_123'.


## Installation & Usage

To install and use the **Convoy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convoy](https://vinkius.com/mcp/convoy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
