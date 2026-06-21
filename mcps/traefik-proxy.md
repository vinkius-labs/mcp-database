# Traefik Proxy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/traefik-proxy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/traefik-proxy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/traefik-proxy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor and manage your Traefik Proxy infrastructure — inspect routers, services, and middlewares directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Traefik Proxy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me an overview of my Traefik proxy status."

**🤖 AI Agent:**
> I've retrieved the overview. You currently have 12 HTTP routers, 8 TCP routers, and 15 services active across 3 entrypoints (web, websecure, and admin).

---

**👤 You:**
> "List all active HTTP routers and their rules."

**🤖 AI Agent:**
> Fetching HTTP routers... I found routers like 'api-rule' (Host(`api.example.com`)) and 'dashboard' (Host(`traefik.internal`)). Would you like to inspect the middlewares for any of these?

---

**👤 You:**
> "Show me the details for the entrypoint named 'websecure'."

**🤖 AI Agent:**
> Inspecting 'websecure'... This entrypoint is listening on address ':443' and has HTTP/3 enabled. It is currently handling traffic for 5 routers.


## Installation & Usage

To install and use the **Traefik Proxy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/traefik-proxy](https://vinkius.com/mcp/traefik-proxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
