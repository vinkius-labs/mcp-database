# Apache APISIX MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apache-apisix)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apache-apisix-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apache-apisix-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your cloud-native API Gateway via AI — configure routes, services, upstreams, and consumers through the APISIX Admin API.

## Description
Connect your **Apache APISIX** instance to any AI agent to orchestrate high-performance traffic management through natural language.

### What you can do

- **Route Orchestration** — List, inspect, create, or delete routes to match client requests and forward them to target upstreams.
- **Service Abstraction** — Manage service entities that group common plugins and upstream configurations for easier API maintenance.
- **Upstream Management** — Configure virtual host abstractions for load balancing, including node management and health checks.
- **Consumer Control** — List and manage API consumers to handle authentication and per-user rate limiting.
- **Configuration as Conversation** — Update complex JSON configurations for any gateway resource without manually using CURL or the Dashboard.

### How it works

1. Subscribe to this server
2. Provide your APISIX Admin URL and Admin Key (X-API-KEY)
3. Start managing your microservices infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly audit routing rules and upstream health directly from the terminal or chat.
- **Backend Developers** — create and test new API routes and service abstractions without leaving the IDE.
- **SRE Teams** — troubleshoot traffic flow and consumer access issues using natural language queries.


## Available Tools
- **dump_control_discovery**: Memory dump of discovered service endpoints
- **dump_control_plugin_metadatas**: Dump all plugin metadata from the Control API
- **dump_control_routes**: Dump all configured Routes from the Control API
- **dump_control_services**: Dump all configured Services from the Control API
- **dump_control_upstreams**: Dump all configured Upstreams from the Control API
- **get_consumer_group**: Get a specific APISIX Consumer Group by ID
- **get_consumer**: Get a specific APISIX Consumer by username
- **get_control_healthcheck**: Get health status of all upstream nodes
- **put_upstream**: Create or update an APISIX Upstream
- **reload_control_plugins**: Trigger a hot reload of plugins
- **trigger_control_gc**: Trigger full garbage collection in the HTTP Lua VM
- **get_control_resource_healthcheck**: Get health status for a specific resource
- **get_control_schema**: Get JSON schemas for all resources and enabled plugins
- **get_global_rule**: Get a specific APISIX Global Rule by ID
- **get_plugin_config**: Get a specific APISIX Plugin Config by ID
- **get_proto**: Get a specific APISIX Proto by ID
- **get_route**: Get a specific APISIX Route by ID
- **get_service**: Get a specific APISIX Service by ID
- **get_ssl**: Get a specific APISIX SSL certificate by ID
- **get_stream_route**: Get a specific APISIX Stream Route by ID
- **get_upstream**: Get a specific APISIX Upstream by ID
- **list_consumer_groups**: List APISIX Consumer Groups
- **list_consumers**: List APISIX Consumers
- **list_global_rules**: List APISIX Global Rules
- **list_plugin_configs**: List APISIX Plugin Configs
- **list_protos**: List APISIX Protos (Protocol Buffers)
- **list_routes**: List APISIX Routes
- **list_services**: List APISIX Services
- **list_ssls**: List APISIX SSL certificates
- **list_stream_routes**: List APISIX Stream Routes (L4 routing)
- **list_upstreams**: List APISIX Upstreams
- **put_consumer_group**: Create or update an APISIX Consumer Group
- **put_consumer**: Create or update an APISIX Consumer
- **put_global_rule**: Create or update an APISIX Global Rule
- **put_plugin_config**: Create or update an APISIX Plugin Config
- **put_proto**: Create or update an APISIX Proto
- **put_route**: Create or update an APISIX Route
- **put_service**: Create or update an APISIX Service
- **put_ssl**: Create or update an APISIX SSL certificate
- **put_stream_route**: Create or update an APISIX Stream Route
- **delete_consumer_group**: Delete an APISIX Consumer Group
- **delete_consumer**: Delete an APISIX Consumer
- **delete_global_rule**: Delete an APISIX Global Rule
- **delete_plugin_config**: Delete an APISIX Plugin Config
- **delete_proto**: Delete an APISIX Proto
- **delete_route**: Delete an APISIX Route
- **delete_service**: Delete an APISIX Service
- **delete_ssl**: Delete an APISIX SSL certificate
- **delete_stream_route**: Delete an APISIX Stream Route
- **delete_upstream**: Delete an APISIX Upstream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apache APISIX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active routes in my APISIX gateway."

**🤖 AI Agent:**
> I've retrieved your routes. You have 3 active routes: 'api-v1' (ID: 1), 'auth-service' (ID: 2), and 'dashboard' (ID: 3). Would you like to see the details for any of them?

---

**👤 You:**
> "Show me the configuration for upstream ID 'backend-cluster'."

**🤖 AI Agent:**
> Fetching upstream 'backend-cluster'... This upstream uses 'roundrobin' balancing with two nodes: 192.168.1.10:8080 (weight 1) and 192.168.1.11:8080 (weight 1).

---

**👤 You:**
> "List all consumers to check who has access to the API."

**🤖 AI Agent:**
> I found 2 consumers: 'mobile-app-client' and 'internal-dev-team'. Both are active and linked to their respective authentication plugins.


## Installation & Usage

To install and use the **Apache APISIX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apache-apisix](https://vinkius.com/mcp/apache-apisix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
