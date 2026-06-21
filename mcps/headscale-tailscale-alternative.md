# Headscale (Tailscale Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/headscale-tailscale-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/headscale-tailscale-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/headscale-tailscale-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage your private Tailscale network via Headscale — control users, nodes, and pre-auth keys directly from your AI agent.

## Description
Connect your self-hosted **Headscale** server to any AI agent and take full control of your private mesh network through natural conversation. Headscale provides an open-source, self-hosted alternative to the Tailscale control server.

### What you can do

- **User Management** — Create, list, and delete administrative users (namespaces) to organize your network segments
- **Node Control** — List all connected machines, fetch detailed metadata for specific nodes, and rename or move them between users
- **Session Security** — Force node expirations or delete machines from the network to revoke access instantly
- **Automated Registration** — Generate and manage pre-auth keys (reusable or ephemeral) to allow new nodes to join without manual approval
- **Route Management** — Inspect and toggle network routes to manage traffic flow across your mesh

### How it works

1. Subscribe to this server
2. Enter your Headscale API Key and Server URL
3. Start managing your infrastructure from Claude, Cursor, or any MCP-compatible client

No more SSH-ing into your controller just to check if a node is online or to generate a registration key. Your AI acts as a network administrator.

### Who is this for?

- **DevOps Engineers** — quickly audit connected nodes and manage namespaces without leaving the terminal or IDE
- **Sysadmins** — automate the lifecycle of VPN nodes and pre-authentication keys for team onboarding
- **Privacy-Conscious Teams** — maintain full control over your self-hosted Tailscale alternative with an AI-powered interface


## Available Tools
- **create_api_key**: Create a new API key
- **create_preauth_key**: Create a new pre-auth key
- **create_user**: Create a new user in Headscale
- **delete_node**: Remove a node from the Headscale network
- **delete_user**: Delete a user from Headscale
- **disable_route**: Disable a specific route
- **enable_route**: Enable a specific route
- **expire_api_key**: Expire an API key
- **expire_node**: Force expiration of a node session
- **expire_preauth_key**: Expire a pre-auth key
- **get_node**: Get details for a specific node
- **list_api_keys**: List all API keys
- **list_nodes**: List all nodes (machines) connected to Headscale
- **list_preauth_keys**: List pre-auth keys
- **list_routes**: List all subnet routes and exit nodes
- **list_users**: List all users in Headscale
- **move_node**: Move a node to a different user
- **rename_node**: Rename a node in Headscale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Headscale (Tailscale Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all nodes currently connected to my Headscale network."

**🤖 AI Agent:**
> I've retrieved the node list. You have 4 active nodes: 'web-server-01' (IP: 100.64.0.1), 'db-primary' (IP: 100.64.0.2), and two others. All are currently online except for 'backup-node'.

---

**👤 You:**
> "Create a new user named 'external-contractors' and generate a reusable pre-auth key for them."

**🤖 AI Agent:**
> User 'external-contractors' has been created successfully. I have also generated a reusable pre-auth key: `hs_auth_...`. This key can be used to register multiple machines under this user.

---

**👤 You:**
> "Get full details for node ID 12 and then expire its session."

**🤖 AI Agent:**
> Inspecting node 12... It's a Linux machine named 'dev-laptop-old'. I have now triggered the `expire_node` action. The machine will be disconnected and will require re-authentication to join the network again.


## Installation & Usage

To install and use the **Headscale (Tailscale Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/headscale-tailscale-alternative](https://vinkius.com/mcp/headscale-tailscale-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
