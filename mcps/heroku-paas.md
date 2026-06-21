# Heroku (PaaS) MCP Server

Manage Heroku apps via AI — list apps, restart dynos, toggle maintenance mode, and audit config vars.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/heroku-paas)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Heroku (PaaS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heroku-paas](https://vinkius.com/mcp/heroku-paas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
