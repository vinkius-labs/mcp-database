# Cloudflare Tunnel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare-tunnel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Cloudflare Tunnels directly from your AI agent — list, create, and configure secure Zero Trust connections to your private infrastructure.

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


## Available Tools (17)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudflare Tunnel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tunnels in my Cloudflare account [ACCOUNT_ID]."

**🤖 AI Agent:**
> I've retrieved your tunnels. You have 3 active tunnels: 'web-server-prod' (Healthy), 'db-bridge' (Healthy), and 'test-lab' (Inactive). Would you like to see the configuration for any of these?

---

**👤 You:**
> "Show me the ingress rules for tunnel [TUNNEL_ID]."

**🤖 AI Agent:**
> Fetching configuration for tunnel [TUNNEL_ID]... The current ingress rules route 'app.example.com' to 'http://localhost:8080' and 'api.example.com' to 'http://localhost:3000'.

---

**👤 You:**
> "Create a new Cloudflare tunnel named 'office-gateway' in account [ACCOUNT_ID]."

**🤖 AI Agent:**
> I've created the tunnel 'office-gateway'. Its ID is [NEW_TUNNEL_ID]. You can now use `get_tunnel_token` to retrieve the token needed to run the connector.


## ❓ FAQ

**Q: Can I update the ingress rules for a remotely managed tunnel?**
Yes. Use the `put_configuration` tool to update the ingress rules and origin request settings for any tunnel that is configured for remote management.

**Q: How do I check if my tunnels are currently online?**
You can use `list_tunnels` with the `status` parameter set to 'healthy' to see active tunnels, or use `get_tunnel` with a specific ID to see its current operational state.

**Q: Can I manage private network routes through this integration?**
Yes. The server includes tools like `list_routes`, `create_route`, and `delete_route` to manage your Cloudflare Tunnel network routing (WARP-to-Tunnel).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare-tunnel](https://vinkius.com/mcp/cloudflare-tunnel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudflare Tunnel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudflare-tunnel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudflare Tunnel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudflare-tunnel": {
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
