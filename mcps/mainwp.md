# MainWP MCP Server

Manage multiple WordPress sites, updates, and security via the MainWP REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mainwp)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 8

## Description
Connect your **MainWP Dashboard** to any AI agent to automate your WordPress network management. This MCP server enables your agent to list child sites, monitor pending updates for core, plugins, and themes, and trigger security scans directly from natural language interfaces.

### What you can do

- **Network Oversight** — List all managed child sites and retrieve real-time status and update counts
- **Update Management** — Query all pending WordPress core, plugin, and theme upgrades across your entire network
- **Automated Sync** — Trigger a global synchronization to fetch the latest data from all connected sites instantly
- **Security Auditing** — Initiate vulnerability scans and malware checks using configured MainWP extensions
- **Inventory Control** — List all plugins and themes installed on any specific child site for auditing
- **One-Click Upgrades** — Execute resource upgrades programmatically to maintain network-wide security

### How it works

1. Subscribe to this server
2. Enter your MainWP Dashboard URL and REST API Bearer Token
3. Ensure 'Pretty Permalinks' are enabled on your WordPress dashboard
4. Start managing your WordPress network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **WordPress Agency Owners** — Monitor client site health and pending updates via simple natural language commands
- **DevOps Engineers** — Automate the synchronization and security scanning of large WordPress networks
- **Site Administrators** — Quickly audit plugin inventories and execute updates without leaving your dev tools


## Available Tools
- **scan_network_malware**: Trigger a malware scan across the network
- **scan_network_vulnerabilities**: Trigger a vulnerability scan across the network
- **list_site_plugins**: List all plugins installed on a specific site
- **list_child_sites**: List all connected WordPress sites
- **sync_child_sites**: Trigger a synchronization with all child sites
- **get_pending_updates_count**: Get a quick count of all pending updates
- **list_available_updates**: List all pending core, plugin, and theme updates
- **upgrade_site_resource**: Requires a JSON body with details.

Execute an upgrade for a specific plugin or theme


## Installation & Usage

To install and use the **MainWP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mainwp](https://vinkius.com/mcp/mainwp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
