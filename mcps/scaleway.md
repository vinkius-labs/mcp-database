# Scaleway MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scaleway)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scaleway-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scaleway-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Scaleway cloud infrastructure — list, create, and control virtual instances directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scaleway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my instances in the Paris zone (fr-par-1)."

**🤖 AI Agent:**
> I've retrieved your instances in fr-par-1. You have 2 active servers: 'web-prod-01' (ID: ...213) and 'db-master' (ID: ...442). Both are currently running.

---

**👤 You:**
> "Create a new DEV1-S instance named 'staging-app' in fr-par-1 using the Ubuntu image."

**🤖 AI Agent:**
> I am initiating the creation of 'staging-app' (DEV1-S) in fr-par-1. The request has been sent to Scaleway, and the instance is now being provisioned.

---

**👤 You:**
> "Reboot the server with ID 550e8400-e29b-41d4-a716-446655440000 in nl-ams-1."

**🤖 AI Agent:**
> The reboot command has been successfully sent to the server in nl-ams-1. It should be restarting now.


## Installation & Usage

To install and use the **Scaleway** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scaleway](https://vinkius.com/mcp/scaleway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
