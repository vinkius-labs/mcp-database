# Dokku MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dokku)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage self-hosted apps via Dokku — monitor containers, scale processes, handle environment variables, and stream logs directly from any AI agent.

## Description
Connect your **Dokku** instance to any AI agent and take full control of your self-hosted PaaS and container orchestration through natural conversation.

### What you can do

- **Application Lifecycle** — List all managed apps and retrieve the overarching directory of deployments on your own infrastructure bypassing standard PaaS fees
- **Provisioning & Deallocation** — Barely instantiate new application repositories or irreversibly dismantle all bound containers and DNS routing records
- **Environment Auditing** — Retrieve the exact `.env` dictionary bound dynamically via the config plugin to observe runtime inputs and SQL credentials
- **Configuration Mutation** — Inject or remove sensitive environment variables securely, triggering rolling app deployments natively across your cluster
- **Process Scaling** — Manipulate explicit replica counts dynamically, determining whether web or worker containers spool up to meet demand
- **Live Log Streaming** — Pull precise system execution tails to investigate explicit request stack traces and crashing node backtraces without SSH
- **One-off Executions** — Launch raw commands inside ephemeral isolated containers for maintenance tasks like DB migrations or custom scripts

### How it works

1. Subscribe to this server
2. Enter your Dokku Host URL and API Token (obtained from your Dokku Pro instance or REST API plugin)
3. Start managing your private cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Indie Hackers & Founders** — manage your self-hosted apps and deploy new versions using natural language
- **DevOps Engineers** — monitor process scales and application health across multiple server nodes
- **SysAdmins** — audit environment variables and verify system logs without manual SSH access
- **Full-stack Developers** — trigger restarts, scale web processes, and run migrations directly from the chat


## Available Tools
- **create_app**: Performs the structural network allocations setting up reverse-proxy hooks (Nginx/Traefik) preceding the actual codebase transfer.

Provision a root App boundary wrapper on the Dokku VM
- **destroy_app**: Instantly shuts down bound running docker containers orchestrating web/worker traffic, detaches volumes seamlessly, and removes explicit DNS routing records from the local VHOST mappings.

Deallocate an App and dismantle all bound containers completely
- **get_logs**: Bypasses SSH to investigate explicit request stack traces, crashing node backtraces, or slow SQL queries happening inside the closed containers.

Stream Dokku Application Docker stdout and stderr logs
- **list_apps**: Determines exactly which Docker containers are orchestrated internally by Dokku Core scaling plugins.

List self-hosted Git-push Apps deployed via Dokku
- **list_config**: env` or `ENV` dictionary bound dynamically via the `dokku config` plugin. Used strictly to observe runtime inputs (SQL credentials, external REST API tokens, Node_ENV bindings) governing app execution.

Extract internal Environment variables loaded into the App
- **ps_restart**: Dokku tears down old running docker processes spanning the App UUID, allocating updated dynamic ports tied via standard proxies (Nginx), ensuring zero downtime deploys if multiple replicas are alive.

Bounce the application container dynamically
- **ps_scale**: Determines whether the "web" container spins zero replicas (suspension), or if "worker" background tasks spool up to 10 endpoints.

Scale structural internal application containers
- **run_command**: Boots a brand new isolated Docker container cloning the production image layers for a single execution cycle. Useful for running `rake db:migrate`, `npm run script` safely disconnected from web traffic.

Launch a raw one-off command inside an ephemeral container
- **set_config**: Triggers a mandatory rolling app deployment unless the `--no-restart` daemon flag applies natively to the process. Critical for updating expired API auth tokens.

Inject Environment Variables into a running Dokku Application
- **unset_config**: Immediately triggers the executing Docker cluster to orchestrate a rapid replacement cycle to strip out the revoked value. Removes stale credentials safely.

Remove sensitive Environment Variables disrupting App config


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dokku** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all apps on my Dokku host"

**🤖 AI Agent:**
> I found 3 apps: 'api-server', 'frontend-web', and 'worker-queue'. All containers are active and managed by the local Docker engine. Would you like to see the config for any of these?

---

**👤 You:**
> "Scale the 'web' process of app 'api-server' to 3 replicas"

**🤖 AI Agent:**
> Scaling request sent! Dokku is now spooling up 3 replicas for the 'web' process of 'api-server'. I will notify you once the internal load balancer has updated the routing.

---

**👤 You:**
> "Get the last 50 lines of logs for 'frontend-web'"

**🤖 AI Agent:**
> Retrieving logs for 'frontend-web'... [Agent pulls precise system execution tails showing request logs, node backtraces, or slow queries happening inside the containers].


## ❓ FAQ

**Q: Can my agent scale my Dokku processes automatically?**
Yes. Use the 'ps_scale' tool. You can specify the application name and the target replica count for processes like 'web' or 'worker'. The agent will manipulate the explicit counts within your Dokku cluster instantly.

**Q: How do I update environment variables via chat?**
Use the 'set_config' tool. Provide the app name, key, and value. The agent will inject the pair into the Docker environment mapping, which typically triggers a rolling deployment to apply the new configuration safely.

**Q: Can I run database migrations through the agent?**
Absolutely. Use the 'run_command' tool. It boots an ephemeral isolated container cloning your production image, allowing you to run maintenance commands like 'rake db:migrate' or custom scripts without affecting live traffic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dokku](https://vinkius.com/mcp/dokku)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dokku** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dokku` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dokku** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dokku": {
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
