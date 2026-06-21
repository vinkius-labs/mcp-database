# ZeroTier MCP Server

Manage ZeroTier virtual networks, authorize members, and monitor local node status directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zerotier)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect your **ZeroTier** infrastructure to any AI agent to orchestrate software-defined networks through natural language. This server bridges the gap between ZeroTier Central management and your local node operations.

### What you can do

- **Central Management** — List all virtual networks and fetch detailed configurations from ZeroTier Central.
- **Member Authorization** — Instantly authorize or de-authorize nodes on your private networks using their Member IDs.
- **Local Node Control** — Check your local node status, version, and address, or join/leave networks directly from your terminal or IDE.
- **Peer Discovery** — List all known peers and network paths to troubleshoot connectivity issues in real-time.
- **Controller Operations** — Manage standalone network controllers and update network configurations programmatically.

### How it works

1. Subscribe to this server
2. Provide your ZeroTier Central API Token (and optionally your local authtoken)
3. Start managing your global area networks from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Automate the provisioning and authorization of new nodes in a secure SD-WAN.
- **Network Administrators** — Monitor network health and peer connectivity without leaving the command line.
- **Remote Teams** — Quickly join or switch between project-specific virtual networks during development.


## Available Tools
- **list_central_network_members**: List all members of a ZeroTier Central network
- **get_central_network**: Get details for a specific ZeroTier Central network
- **list_central_networks**: List all ZeroTier Central networks
- **update_central_network_member**: Update a member configuration in a ZeroTier Central network
- **list_controller_network_members**: List members of a managed network on the local controller
- **list_controller_networks**: List all networks managed by the local controller
- **update_controller_network_member**: Authorize or configure a member on the local controller
- **update_controller_network**: Create or update a network configuration on the local controller
- **join_local_network**: Join a ZeroTier network locally
- **leave_local_network**: Leave a ZeroTier network locally
- **list_local_networks**: List networks the local ZeroTier node is a member of
- **list_local_peers**: List all known ZeroTier peers locally
- **get_local_status**: Get local ZeroTier node status


## Installation & Usage

To install and use the **ZeroTier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerotier](https://vinkius.com/mcp/zerotier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
