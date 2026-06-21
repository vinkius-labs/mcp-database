# MainWP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mainwp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mainwp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mainwp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage multiple WordPress sites, updates, and security via the MainWP REST API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MainWP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all connected child sites in MainWP."

**🤖 AI Agent:**
> I've retrieved your sites. You have 12 active child sites, including 'Corporate Blog', 'Client E-shop', and 'Portfolio Site'. Would you like to check for pending updates?

---

**👤 You:**
> "How many pending updates are available across my network?"

**🤖 AI Agent:**
> There are currently 45 updates available: 2 for WordPress core, 35 for plugins, and 8 for themes across your entire network.

---

**👤 You:**
> "Run a vulnerability scan across all sites."

**🤖 AI Agent:**
> I've initiated the network-wide vulnerability scan. MainWP is now checking for known issues in your plugins and themes. I will notify you once the process is complete.


## Installation & Usage

To install and use the **MainWP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mainwp](https://vinkius.com/mcp/mainwp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
