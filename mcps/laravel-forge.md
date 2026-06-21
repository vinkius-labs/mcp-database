# Laravel Forge MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/laravel-forge)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/laravel-forge-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/laravel-forge-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Laravel Forge servers, orchestrate site deployments, and query databases directly from your AI agent.

## Description
Connect your **Laravel Forge** developer account to an AI agent to execute complex devops tasks natively in chat.

### What you can do

- **Server Ecosystems** — List all connected drops, inspect internal structures, and check status
- **Deployments** — Safely dispatch site deployment scripts and watch output structures
- **Database Configurations** — Query connected DB clusters linked to given domains
- **Worker Operations** — Expose active daemon configurations routing jobs under your servers

### How it works

1. Subscribe dynamically to this endpoint
2. Provide your core Laravel Forge API token string
3. Engage your new devops engineer via Cursor or Claude

### Who is this for?

- **DevOps Engineers** — run deployments natively through chat commands during sprint reviews
- **Lead Developers** — instantly check worker and SSH key metadata safely tracked inside Forge environments
- **System Admins** — audit entire physical networks executing zero shell scripts


## Available Tools
- **deploy_site**: Command a deployment script queue to execute on a repository site
- **get_server**: Retrieve detailed data on a specific server droplet
- **get_site**: Look up specifics for an exact site layout on a server
- **list_databases**: List active databases mounted on a Forge server
- **list_recipes**: Retrieve available custom shell recipes within your organizational team limits
- **list_servers**: Retrieve the master list of all connected Forge servers
- **list_sites**: List websites mounted to a specific server
- **list_ssh_keys**: Retrieve active physical access keys inserted on the root server
- **list_workers**: Retrieve queue worker configurations executing on a tracked site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laravel Forge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Display all the cloud server instances operating in the fleet."

**🤖 AI Agent:**
> Here's what I observed... You have 2 droplets attached: 'Production Web' and 'Staging Loadbalancer'. Should I probe their sites?

---

**👤 You:**
> "Deploy the pending commits directly to staging site 5210 on server 1205."

**🤖 AI Agent:**
> Deploying package payload... Success! Forge emitted a validation flag kicking off the repository deployment routine on site 5210.

---

**👤 You:**
> "Check the active workers running on the production server."

**🤖 AI Agent:**
> Scanning worker processes... Found 2 active Queue workers on the Production Server handling redis payloads securely.


## Installation & Usage

To install and use the **Laravel Forge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/laravel-forge](https://vinkius.com/mcp/laravel-forge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
