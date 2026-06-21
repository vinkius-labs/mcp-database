# Traefik Proxy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/traefik-proxy)
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


## Available Tools (18)
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


## ❓ FAQ

**Q: Can I see the full runtime configuration of my Traefik instance?**
Yes. Use the `get_rawdata` tool to retrieve the entire runtime configuration, including all providers, routers, services, and middlewares in a single response.

**Q: How do I check the status of a specific HTTP service?**
You can use `list_http_services` to see all services or `get_http_service` with the specific service name to get detailed health and configuration metrics.

**Q: Does this support TCP and UDP routing inspection?**
Absolutely. The server includes dedicated tools like `list_tcp_routers`, `list_udp_routers`, and their corresponding service tools to manage non-HTTP traffic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/traefik-proxy](https://vinkius.com/mcp/traefik-proxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Traefik Proxy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `traefik-proxy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Traefik Proxy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "traefik-proxy": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
