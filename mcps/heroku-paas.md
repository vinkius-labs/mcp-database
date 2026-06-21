# Heroku (PaaS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heroku-paas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Heroku apps via AI — list apps, restart dynos, toggle maintenance mode, and audit config vars.

## Description
Connect your **Heroku** account to any AI agent and take full control of your cloud-native application management and dyno orchestration through natural conversation.

### What you can do

- **App Management** — List all hosted applications, create new deployment boundaries, and fetch intricate runtime constraints and framework details directly from your agent
- **Dyno Orchestration** — List individual containerized dynos, track their status (up, crashed, idle), and selectively reboot specific instances or entire clusters
- **Environment & Config** — Audit decrypted application environment variables (Config Vars) and retrieve third-party platform add-ons like Postgres or Redis
- **Operational Control** — Rapidly toggle maintenance mode to block inbound requests during migrations and perform hard reboots on stalled application clusters
- **Infrastructure Audit** — Identify underlying executing stacks (e.g. heroku-24), regional datacenter placements (US/EU), and total slug size in memory

### How it works

1. Subscribe to this server
2. Enter your Heroku API Key
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor dyno health and perform rolling restarts or cluster reboots through natural conversation
- **Backend Developers** — check environment variables, add-on statuses, and deployment regions without leaving your IDE or switching to the dashboard
- **System Admins** — manage maintenance windows and application lifecycles across multiple environments and regions efficiently


## Available Tools
- **create_app**: Provision a fresh structural App container on Heroku
- **delete_app**: Traffic routing instantly yields persistent 404/no web-dynos responses. Highly destructive.

Permanently wipe an active App from Heroku servers
- **get_app_info**: g. heroku-22, heroku-24). Confirms exact application routing URL mapping, total slug (code) size in memory, and regional datacenter placements (US or EU) verifying global latency strategies.

Fetch intricate runtime constraints and framework details of an App
- **list_addons**: Retrieve third-party Platform Add-ons mapping to an App
- **list_apps**: Use this to discover App IDs, web URL designations, and git repository targets required to execute operational commands downstream.

List all standard applications actively hosted on Heroku PaaS
- **list_dynos**: 1, worker.1). Tracks exactly whether the dyno is "up", "crashed", "idle", or "starting" based on the internal slug runner engine's telemetry.

List discrete containerized Dynos executing inside an App
- **list_config_vars**: Retrieves highly confidential database tokens `DATABASE_URL`, SendGrid passwords, or OAuth keys.

Dump decrypted Application Environment Variables
- **restart_specific_dyno**: Exceedingly useful for unsticking hung asynchronous queue workers without impacting active web traffic on the primary frontend replicas.

Selectively reboot one isolated Dyno instance (e.g. worker.2)
- **restart_all_dynos**: Often resolves ephemeral memory-leaks in Node.js or Ruby runtimes stalling standard request processing.

Hard reboot all containers tied to an entire Application
- **toggle_maintenance_mode**: Crucial for orchestrating complex sequential database migrations without encountering corrupted states from active sessions.

Rapidly switch an Application's Maintenance Mode switch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heroku (PaaS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Heroku apps"

**🤖 AI Agent:**
> I've found 4 applications: 'production-api', 'staging-web', 'worker-service', and 'data-pipeline'. Which one would you like to inspect?

---

**👤 You:**
> "Restart all dynos for 'production-api'"

**🤖 AI Agent:**
> Restarting all dynos for 'production-api'… All web and worker containers are being recycled. This should resolve any transient issues within the next minute.

---

**👤 You:**
> "What's the current maintenance mode status for the 'staging-web' app?"

**🤖 AI Agent:**
> Maintenance mode is currently DISABLED for 'staging-web'. Would you like to enable it before performing your database migration?


## ❓ FAQ

**Q: Can I see the status of my dynos through my agent?**
Yes. Use the `list_dynos` tool to see the real-time status of each container process (e.g. web.1, worker.1). You'll know exactly if a dyno is up, crashed, starting, or idle.

**Q: How do I check my application's environment variables?**
The `list_config_vars` tool allows your agent to dump the full dictionary of environment variables injected into your dynos, including sensitive keys like DATABASE_URL or API tokens.

**Q: Can my agent restart a specific hung worker without affecting the web traffic?**
Absolutely. Use the `restart_specific_dyno` tool to reboot a single instance (e.g. worker.2). This is perfect for unsticking hung asynchronous queue workers without impacting your primary frontend traffic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heroku-paas](https://vinkius.com/mcp/heroku-paas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heroku (PaaS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `heroku-paas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heroku (PaaS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heroku-paas": {
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
