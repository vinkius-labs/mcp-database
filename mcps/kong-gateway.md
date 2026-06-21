# Kong Gateway MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kong-gateway)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kong-gateway-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kong-gateway-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Manage your API Gateway infrastructure — list services, configure routes, and manage consumers or plugins directly from any AI agent.

## Description
Connect your **Kong Gateway** Admin API to any AI agent and take full control of your API management lifecycle through natural conversation.

### What you can do

- **Services & Routes** — List, create, and update upstream services and their associated routing rules to manage traffic flow.
- **Consumer Management** — Query and manage API consumers, allowing you to track users and applications interacting with your gateway.
- **Plugin Configuration** — Inspect and manage plugins for authentication, rate limiting, and logging across your services and routes.
- **Upstreams & Targets** — Configure load balancing by managing upstreams and their health-checked targets.
- **SSL/TLS Management** — List and update certificates and SNIs to ensure secure communication across your endpoints.
- **System Health** — Retrieve real-time status and information about your Kong instance to monitor performance.

### How it works

1. Subscribe to this server
2. Enter your Kong Admin URL (and optional Admin Token)
3. Start managing your API infrastructure from Claude, Cursor, or any MCP-compatible client

No more manual cURL commands or navigating complex dashboards to check a route configuration. Your AI acts as a dedicated DevOps engineer or API Architect.

### Who is this for?

- **DevOps Engineers** — quickly check gateway status, list plugins, and verify upstream health without leaving the terminal or IDE.
- **Backend Developers** — create and test new services and routes instantly during the development cycle.
- **API Architects** — audit consumer access and plugin configurations to ensure security and compliance across the organization.


## Available Tools
- **create_certificate**: Create a new Kong Certificate
- **create_consumer**: Create a new Kong Consumer
- **create_plugin**: Create a new Kong Plugin
- **create_route**: Create a new Kong Route
- **create_service**: Create a new Kong Service
- **create_sni**: Create a new Kong SNI
- **create_target**: Create a new Target for an Upstream
- **create_upstream**: Create a new Kong Upstream
- **delete_certificate**: Delete a Kong Certificate
- **delete_consumer**: Delete a Kong Consumer
- **delete_plugin**: Delete a Kong Plugin
- **delete_route**: Delete a Kong Route
- **delete_service**: Delete a Kong Service
- **delete_sni**: Delete a Kong SNI
- **delete_target**: Delete a Target from an Upstream
- **delete_upstream**: Delete a Kong Upstream
- **get_certificate**: Get details for a specific Kong Certificate
- **get_consumer**: Get details for a specific Kong Consumer
- **get_info**: Retrieve general information about the Kong node
- **get_plugin**: Get details for a specific Kong Plugin
- **get_route**: Get details for a specific Kong Route
- **get_service**: Get details for a specific Kong Service
- **get_sni**: Get details for a specific Kong SNI
- **get_status**: Retrieve the status of the Kong node
- **get_upstream**: Get details for a specific Kong Upstream
- **list_certificates**: List all Kong Certificates
- **list_consumers**: List all Kong Consumers
- **list_plugins**: List all Kong Plugins
- **list_routes**: List all Kong Routes
- **list_services**: List all Kong Services
- **list_snis**: List all Kong SNIs
- **list_targets**: List all Targets for an Upstream
- **list_upstreams**: List all Kong Upstreams
- **update_certificate**: Update an existing Kong Certificate
- **update_consumer**: Update an existing Kong Consumer
- **update_plugin**: Update an existing Kong Plugin
- **update_route**: Update an existing Kong Route
- **update_service**: Update an existing Kong Service
- **update_sni**: Update an existing Kong SNI
- **update_upstream**: Update an existing Kong Upstream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kong Gateway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all services currently configured in Kong."

**🤖 AI Agent:**
> I've retrieved the services. You have 3 services configured: 'billing-api', 'users-service', and 'inventory-proxy'. Would you like to see the details for any of them?

---

**👤 You:**
> "Create a new service named 'auth-api' pointing to 'http://auth.internal'."

**🤖 AI Agent:**
> Service 'auth-api' has been successfully created with ID '8273-abc-123'. It is configured to point to 'http://auth.internal' on port 80. Should I create a route for this service now?

---

**👤 You:**
> "What is the current status of my Kong Gateway node?"

**🤖 AI Agent:**
> The Kong node is healthy. Database is reachable, and there are currently 124 active connections. The server has been up for 14 days.


## Installation & Usage

To install and use the **Kong Gateway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kong-gateway](https://vinkius.com/mcp/kong-gateway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
