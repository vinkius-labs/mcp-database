# Vultr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vultr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vultr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vultr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Vultr cloud infrastructure, bare metal instances, and backups directly from your AI agent.

## Description
Connect your **Vultr** account to any AI agent to manage your cloud infrastructure through natural conversation.

### What you can do

- **Bare Metal Management** — List, create, start, reboot, and delete physical hardware instances across global regions.
- **Account & Networking** — Retrieve account info, billing status, BGP configurations, and manage IPv4/IPv6 reverse DNS settings.
- **Backups & Apps** — List automated backups and browse the Vultr Marketplace for one-click application deployments.
- **API Key Control** — List and create API keys to manage access levels for your infrastructure programmatically.
- **Instance Lifecycle** — Perform critical operations like reinstalling or halting bare metal servers directly from your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Vultr API Key
3. Start managing your high-performance infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check server statuses and reboot bare metal instances without leaving the terminal or IDE.
- **Cloud Architects** — inspect BGP settings and network configurations across multiple regions.
- **Developers** — browse and deploy marketplace applications or manage API keys for automated workflows.


## Available Tools
- **get_bare_metal_ipv6**: Get IPv6 info for a bare metal instance
- **halt_bare_metal**: Halt a bare metal instance
- **reboot_bare_metal**: Reboot a bare metal instance
- **reinstall_bare_metal**: Reinstall a bare metal instance
- **set_bare_metal_ipv4_reverse**: Set Reverse DNS for IPv4 on a bare metal instance
- **set_bare_metal_ipv6_reverse**: Set Reverse DNS for IPv6 on a bare metal instance
- **setup_bgp**: Setup BGP for the account
- **start_bare_metal**: Start a bare metal instance
- **delete_bare_metal**: Delete a bare metal instance
- **list_backups**: List backups
- **list_bare_metals**: List bare metal instances
- **create_api_key**: Create a new API key
- **get_bare_metal_ipv4**: Get IPv4 info for a bare metal instance
- **get_backup**: Get a specific backup
- **create_bare_metal**: Create a bare metal instance
- **get_account_bgp**: Get Account BGP Info
- **get_account**: Get Vultr account info
- **list_api_keys**: List API keys
- **list_applications**: List Vultr applications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vultr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bare metal instances."

**🤖 AI Agent:**
> I've retrieved your bare metal instances. You have 2 active servers: 'DB-Primary' (ID: 550e8400) in New Jersey and 'Web-Frontend' (ID: 660f9511) in Tokyo. Would you like to see the IP details for one of them?

---

**👤 You:**
> "Show my Vultr account and billing information."

**🤖 AI Agent:**
> Your account is currently active with a balance of $45.20. Your registered email is 'admin@example.com' and the account is in good standing. Would you like to check your BGP status as well?

---

**👤 You:**
> "What marketplace applications are available for deployment?"

**🤖 AI Agent:**
> I've listed the available applications. You can deploy 'Docker', 'WordPress', 'cPanel', or 'LAMP' as one-click apps, or choose from various Marketplace images like 'Plesk' or 'OpenVPN'. Which one would you like to deploy?


## Installation & Usage

To install and use the **Vultr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vultr](https://vinkius.com/mcp/vultr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
