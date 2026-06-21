# Traefik Proxy MCP Server

Monitor and manage your Traefik Proxy infrastructure — inspect routers, services, and middlewares directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/traefik-proxy)

## Overview
**Category:** loved-by-devs
**Tools Count:** 18

## Description
Connect your **Traefik Proxy** instance to any AI agent and gain real-time visibility into your edge router configuration through natural conversation.

### What you can do

- **System Overview** — Get a high-level summary of your Traefik state, including the count of active routers, services, and entrypoints.
- **HTTP/TCP/UDP Inspection** — List and drill down into specific routers and services across all supported protocols.
- **Middleware Analysis** — Inspect middleware configurations to understand how requests are being transformed or secured.
- **Entrypoint Mapping** — View all configured entrypoints and their current status to troubleshoot network access.
- **Raw Configuration** — Access the full runtime configuration for deep debugging and infrastructure auditing.

### How it works

1. Subscribe to this server
2. Provide your Traefik API URL (ensure the API is enabled in your Traefik config)
3. (Optional) Provide Basic Auth credentials if your API is protected
4. Start auditing your infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly verify routing rules and service health without accessing the Traefik dashboard
- **Backend Developers** — check if new services are correctly discovered and middlewares are applied
- **SRE Teams** — audit the entire proxy configuration to ensure security standards and entrypoint consistency


## Available Tools
- **get_entrypoint**: Get details for a specific entrypoint
- **get_http_middleware**: Get details for a specific HTTP middleware
- **get_http_router**: Get details for a specific HTTP router
- **get_http_service**: Get details for a specific HTTP service
- **get_tcp_middleware**: Get details for a specific TCP middleware
- **get_tcp_router**: Get details for a specific TCP router
- **get_tcp_service**: Get details for a specific TCP service
- **list_entrypoints**: List all entrypoints
- **list_http_middlewares**: List all HTTP middlewares
- **list_http_routers**: List all HTTP routers
- **list_http_services**: List all HTTP services
- **list_tcp_middlewares**: List all TCP middlewares
- **list_tcp_routers**: List all TCP routers
- **list_tcp_services**: List all TCP services
- **list_udp_routers**: List all UDP routers
- **list_udp_services**: List all UDP services
- **get_overview**: ).

Get Traefik overview
- **get_rawdata**: Get Traefik raw runtime configuration


## Installation & Usage

To install and use the **Traefik Proxy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/traefik-proxy](https://vinkius.com/mcp/traefik-proxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
