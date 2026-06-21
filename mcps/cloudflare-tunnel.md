# Cloudflare Tunnel MCP Server

Manage Cloudflare Tunnels directly from your AI agent — list, create, and configure secure Zero Trust connections to your private infrastructure.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare-tunnel)

## Overview
**Category:** industry-titans
**Tools Count:** 17

## Description
Connect your **Cloudflare** account to any AI agent to take full control of your Zero Trust connectivity and private network routing through natural conversation.

### What you can do

- **Tunnel Management** — List all tunnels in your account, filter by status (healthy, degraded, down), and fetch detailed metadata for specific tunnels.
- **Remote Configuration** — Retrieve and update ingress rules and origin settings for remotely-managed tunnels without touching the CLI.
- **Network Routing** — Manage private network routes (CIDR) and IP-based routing to connect your internal resources securely.
- **Connection Monitoring** — Inspect active connectors, list tunnel connections, and clean up stale sessions to ensure high availability.
- **Lifecycle Actions** — Create new tunnels, update secrets, or delete decommissioned tunnels directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Cloudflare API Token (with Cloudflare Tunnel permissions)
3. Start managing your secure tunnels from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check tunnel health and update ingress rules during deployments without leaving the terminal or IDE.
- **Security Teams** — audit active tunnels and network routes to ensure compliance with Zero Trust policies.
- **System Administrators** — automate the cleanup of stale connections and monitor the status of remote connectors across multiple accounts.


## Available Tools
- **cleanup_connections**: If no client_id is provided, all connectors are removed.

Clean up Cloudflare Tunnel connections
- **create_route**: Create a tunnel route
- **create_tunnel**: Create a new Cloudflare Tunnel
- **delete_route**: Delete a tunnel route
- **delete_tunnel**: Delete a Cloudflare Tunnel
- **get_configuration**: Get configuration for a remotely-managed tunnel
- **get_connector**: Get Cloudflare Tunnel connector details
- **get_management_token**: Get a Cloudflare Tunnel management token
- **get_route_by_ip**: Get tunnel route by IP
- **get_tunnel_token**: Get a Cloudflare Tunnel token
- **get_tunnel**: Get details for a single Cloudflare Tunnel
- **list_connections**: List Cloudflare Tunnel connections
- **list_routes**: List tunnel routes
- **list_tunnels**: List and filter Cloudflare Tunnels in an account
- **put_configuration**: Add or update configuration for a remotely-managed tunnel
- **update_route**: Update a tunnel route
- **update_tunnel**: Update an existing Cloudflare Tunnel


## Installation & Usage

To install and use the **Cloudflare Tunnel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare-tunnel](https://vinkius.com/mcp/cloudflare-tunnel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
