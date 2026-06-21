# zrok (Open-Source Tunnel) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zrok-open-source-tunnel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Securely share local resources with the world using zrok — manage environments, create public/private shares, and monitor tunnels directly from your AI agent.

## Description
Connect your **zrok** account to any AI agent to orchestrate secure tunnels and sharing workflows through natural language. zrok is an open-source sharing platform built on OpenZiti.

### What you can do

- **Environment Control** — Enable or disable environments to register your machines and containers with the zrok controller.
- **Instant Sharing** — Create public or private shares for your local services (HTTP, TCP, UDP) with a single command.
- **Tunnel Management** — List all active shares, retrieve specific share details, and delete tunnels when they are no longer needed.
- **Account Overview** — Monitor your account status, usage limits, and active environments to maintain full visibility.

### How it works

1. Subscribe to this server
2. Enter your zrok Account Token
3. Start exposing local services securely from Claude, Cursor, or any MCP client

No more manual CLI commands to check if your tunnel is still up. Your AI acts as a network administrator.

### Who is this for?

- **Developers** — instantly expose local dev servers for testing or webhooks without complex firewall rules.
- **DevOps Engineers** — manage and monitor remote environments and shares across multiple machines.
- **Security Teams** — utilize private sharing modes to grant access to internal resources securely.


## Available Tools
- **get_account**: Get account details and limits
- **create_share**: ).

Create a new share (public or private)
- **delete_share**: Delete a share
- **disable_environment**: Disable an environment
- **enable_environment**: Enable a new environment
- **get_share**: Get details for a specific share
- **list_environments**: List all enabled environments
- **list_shares**: List all active shares
- **login_account**: Authenticate and receive a token
- **register_account**: Register a new zrok account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **zrok (Open-Source Tunnel)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the environments enabled on my zrok account."

**🤖 AI Agent:**
> I've retrieved your environments. You have 2 active environments: 'MacBook-Pro-Local' (Token: env_abc123) and 'Ubuntu-Server-Prod' (Token: env_xyz789).

---

**👤 You:**
> "Create a public proxy share for my local port 8000."

**🤖 AI Agent:**
> Creating share... Done! Your local service at http://localhost:8000 is now publicly accessible at https://random-name.share.zrok.io. The share token is 'sh_98765'.

---

**👤 You:**
> "Check my zrok account status and limits."

**🤖 AI Agent:**
> Fetching account details... Your account is active. You are currently using 3 out of 10 allowed environments and 5 out of 20 allowed shares. Your data transfer for this period is at 15%.


## ❓ FAQ

**Q: How do I create a public tunnel for my local web server?**
Use the `create_share` tool. Specify the `backend` (e.g., http://localhost:8080), set `share_mode` to 'public', and `backend_mode` to 'proxy'. The agent will return the public URL.

**Q: Can I see all my currently active tunnels across all environments?**
Yes! Run the `list_shares` tool. It will retrieve a list of all active shares associated with your account, including their tokens and backend configurations.

**Q: How do I stop an environment from being active in zrok?**
You can use the `disable_environment` tool. This will remove the environment registration from the zrok controller, effectively disconnecting that machine or container.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zrok-open-source-tunnel](https://vinkius.com/mcp/zrok-open-source-tunnel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **zrok (Open-Source Tunnel)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zrok-open-source-tunnel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **zrok (Open-Source Tunnel)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zrok-open-source-tunnel": {
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
