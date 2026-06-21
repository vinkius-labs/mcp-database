# Tailscale MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tailscale)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tailscale-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tailscale-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your Tailscale mesh network — list devices, update ACL policies, manage auth keys, and inspect users directly from any AI agent.

## Description
Connect your **Tailscale** network (tailnet) to any AI agent and take full control of your zero-trust infrastructure through natural conversation.

### What you can do

- **Device Management** — List all nodes in your tailnet, fetch specific device details, authorize new machines, or update device tags to organize your fleet.
- **Network Security (ACLs)** — Retrieve and update your HuJSON policy files (ACLs) to manage access control without leaving your chat interface.
- **Authentication Keys** — List, create, and delete auth keys to automate node joining or manage ephemeral server access.
- **User Auditing** — List all users within your tailnet and fetch detailed profile information for specific members.
- **Node Cleanup** — Securely delete decommissioned devices from your tailnet using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Tailscale API Key
3. Start managing your private network from Claude, Cursor, or any MCP-compatible client

No more jumping between the Tailscale admin console and your terminal. Your AI acts as a network administrator that understands your infrastructure context.

### Who is this for?

- **DevOps Engineers** — quickly check node statuses, manage tags, and generate auth keys for CI/CD pipelines.
- **Security Teams** — audit tailnet users and inspect or update ACL policies to ensure zero-trust compliance.
- **IT Administrators** — authorize new devices and clean up old nodes from the network via simple commands.


## Available Tools
- **authorize_device**: Authorize Device
- **create_auth_key**: Create Auth Key
- **delete_auth_key**: Delete Auth Key
- **delete_device**: Delete Device
- **get_tailnet_acl**: Get Tailnet Policy (ACL)
- **get_auth_key**: Get Auth Key
- **get_device**: Get Device Details
- **get_user**: Get User
- **list_auth_keys**: List Auth Keys
- **list_tailnet_devices**: List Tailnet Devices
- **list_users**: List Users
- **update_tailnet_acl**: Update Tailnet Policy (ACL)
- **update_device_tags**: Update Device Tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailscale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all devices in the tailnet 'mycompany.com'."

**🤖 AI Agent:**
> I've retrieved the device list for mycompany.com. You have 12 active nodes, including 'web-server-01' (ID: 14023) and 'dev-laptop' (ID: 15092). Would you like details on a specific one?

---

**👤 You:**
> "Show me the current ACL policy for my default tailnet."

**🤖 AI Agent:**
> Fetching the HuJSON policy... Here is your current ACL. It defines 5 groups and 12 access rules. Would you like me to help you update any specific rule?

---

**👤 You:**
> "Create a new reusable auth key for the tailnet 'example.com'."

**🤖 AI Agent:**
> I've created a new reusable auth key for example.com. The key ID is 'key-abc123xyz'. Please make sure to store it securely as it won't be shown again.


## Installation & Usage

To install and use the **Tailscale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tailscale](https://vinkius.com/mcp/tailscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
