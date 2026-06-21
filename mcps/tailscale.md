# Tailscale MCP Server

Manage your Tailscale mesh network — list devices, update ACL policies, manage auth keys, and inspect users directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tailscale)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

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


## Installation & Usage

To install and use the **Tailscale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tailscale](https://vinkius.com/mcp/tailscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
