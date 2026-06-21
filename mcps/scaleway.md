# Scaleway MCP Server

Manage Scaleway cloud infrastructure — list, create, and control virtual instances directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/scaleway)

## Overview
**Category:** developer-tools
**Tools Count:** 3

## Description
Connect your **Scaleway** account to any AI agent to manage your cloud infrastructure through natural language. This server provides direct access to the Scaleway Instances API.

### What you can do

- **Instance Discovery** — List all virtual machines across different availability zones (e.g., fr-par-1, nl-ams-1)
- **Provisioning** — Create new instances by specifying names, commercial types (like DEV1-S), and image IDs
- **Power Management** — Remotely power on, power off, or reboot your servers
- **Lifecycle Control** — Terminate instances that are no longer needed directly from the chat

### How it works

1. Subscribe to this server
2. Enter your Scaleway Secret Key
3. Start managing your cloud resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check server status or reboot instances without leaving the terminal or IDE
- **Developers** — spin up new development environments using simple text commands
- **Cloud Architects** — audit active resources across multiple zones efficiently


## Available Tools
- **create_instance**: Create a new Scaleway instance (server)
- **perform_instance_action**: Perform an action on a Scaleway instance (e.g., poweron, poweroff)
- **list_instances**: List Scaleway instances (servers) in a specific zone


## Installation & Usage

To install and use the **Scaleway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scaleway](https://vinkius.com/mcp/scaleway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
