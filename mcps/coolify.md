# Coolify MCP Server

Manage self-hosting via Coolify — monitor servers, deploy applications, manage databases, and trigger builds directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coolify)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Coolify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coolify](https://vinkius.com/mcp/coolify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
