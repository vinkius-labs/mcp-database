# Dokku MCP Server

Manage self-hosted apps via Dokku — monitor containers, scale processes, handle environment variables, and stream logs directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dokku)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Dokku** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dokku](https://vinkius.com/mcp/dokku)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
