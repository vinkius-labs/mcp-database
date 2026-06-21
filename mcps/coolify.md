# Coolify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coolify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage self-hosting via Coolify — monitor servers, deploy applications, manage databases, and trigger builds directly from any AI agent.

## Description
Connect your **Coolify** instance to any AI agent and take full control of your self-hosting and private cloud workflows through natural conversation.

### What you can do

- **Server Monitoring** — List self-hosted nodes and retrieve intricate networking parameters including IP properties and Docker swarm statuses
- **Application Management** — List all managed frontend/backend apps and fetch elaborate internal topology metrics like mapped GitHub branches and Traefik proxy paths
- **Lifecycle Control** — Start, stop, and restart applications natively, allowing you to recycle container states and apply configuration updates instantly
- **Deployment Automation** — Trigger raw build pipelines to fetch the latest commits, rebuild Nixpacks images, and roll out updated Docker versions
- **Database Oversight** — Manage PostgreSQL, MySQL, and Redis configurations and extrapolate internal connection strings for secure application linking
- **Resource Navigation** — asociating Project repositories to explicit application UUIDs required for downstream mutations and operational auditing

### How it works

1. Subscribe to this server
2. Enter your Coolify Instance URL and API Token (found in Keys & Tokens > API Tokens)
3. Start managing your self-hosted cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Indie Hackers & Founders** — manage your private cloud and deploy new versions without touching the dashboard
- **DevOps Engineers** — monitor server node health and application lifecycle states across multiple environments
- **Full-stack Developers** — trigger builds, restart containers, and retrieve database connection strings directly from the chat
- **SysAdmins** — audit Docker Swarm configurations and verify server connectivity through natural language


## Available Tools
- **get_application**: Examines mapped GitHub branches, automatic rollout toggles (push to deploy), and assigned Traefik reverse proxy FQDN paths.

Fetch elaborate internal topology metrics for a given Application
- **get_database**: Highly required when linking newly provisioned Web Apps to Backend Datastores.

Extrapolate internal configuration arrays for a Database
- **get_server**: Verifies IP properties, SSH connection validation statuses, and Docker executing ports resolving across the cluster.

Get configuration schema mapped to a specific Coolify Server Node
- **list_applications**: Generates the crucial map associating Project repositories to explicit application UUIDs required for downstream mutations (like restarting and stopping).

List all frontend/backend Applications actively managed by Coolify
- **list_databases**: Isolates database bounding boxes mapping to applications so you can properly retrieve Connection Strings and backup cadence timelines.

List managed PostgreSQL, MySQL, and Redis configurations
- **list_servers**: Used to identify the raw physical endpoints running Docker swarms that host subsequent applications.

List all self-hosted Server Nodes attached to Coolify
- **restart_application**: Ensures updated config `.env` variables injected via Coolify take effect immediately in runtime RAM.

Bounce a Coolify application recycling its container states
- **start_application**: Spin up containers mapped to a suspended Application UUID
- **stop_application**: Used precisely for pausing billing or restricting web perimeter ingress during a cyber incident directly via the Coolify dashboard API.

Halt execution algorithms suspending the mapped Application
- **trigger_deployment**: Performs `git fetch`, rebuilds Nixpacks images, caches dependencies, and rolls the updated Docker image out directly over the previous active application version.

Trigger a raw build pipeline fetching the latest Git commit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coolify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active servers in my Coolify instance"

**🤖 AI Agent:**
> I found 2 servers: 'Main-Hetzner-Node' (UUID: abc-123) and 'Backup-Vultr' (UUID: def-456). Both are connected and running Docker Swarm. Would you like to see the applications on either of these?

---

**👤 You:**
> "Trigger a deployment for application 'backend-api'"

**🤖 AI Agent:**
> Deployment triggered for 'backend-api'! Coolify is now fetching the latest Git commit and rebuilding the Nixpacks image. I will notify you once the new version is live.

---

**👤 You:**
> "What is the connection string for database 'user-db-prod'?"

**🤖 AI Agent:**
> Retrieving connection string for 'user-db-prod'... The internal URI is: postgres://user:pass@coolify-db-abc:5432/user_db. This URI is only accessible within your internal Docker network.


## ❓ FAQ

**Q: Can my agent trigger a new deployment for a Coolify application?**
Yes. Use the 'trigger_deployment' tool with the application UUID. The agent will initiate a full build pipeline, fetching the latest commit and rolling out the updated version directly on your server.

**Q: How do I retrieve the internal connection string for a managed database?**
Provide the database UUID to the 'get_database' tool. Your agent will extrapolate the internal network URI (e.g., for PostgreSQL or MySQL), allowing you to securely link your apps without external port exposure.

**Q: Can I restart an application to apply new environment variables?**
Absolutely. Use the 'restart_application' tool. The agent will execute an overlapping bounce, destroying old instances and initializing fresh replicas with the latest configuration and environment variables.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coolify](https://vinkius.com/mcp/coolify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coolify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coolify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coolify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coolify": {
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
