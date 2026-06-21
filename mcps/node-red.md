# Node-RED MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/node-red)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/node-red-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/node-red-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Node-RED flows, nodes, and system diagnostics directly from your AI agent.

## Description
Connect your **Node-RED** instance to any AI agent to orchestrate your event-driven applications and IoT workflows through natural language.

### What you can do

- **Flow Management** — Retrieve, create, update, or delete entire flow configurations and individual tabs using `get_flows`, `add_flow`, and `delete_flow`.
- **Node Operations** — List all installed node modules and dynamically install or remove npm packages with `install_node` and `remove_node`.
- **System Diagnostics** — Monitor runtime health, including OS details, Node.js version, and memory usage via `get_diagnostics`.
- **Configuration Control** — Fetch runtime settings and user information to understand your environment's constraints.

### How it works

1. Subscribe to this server
2. Provide your Node-RED Base URL and Access Token
3. Start automating your low-code environment from Claude, Cursor, or any MCP client

### Who is this for?

- **IoT Developers** — monitor and modify edge computing flows without leaving the terminal or editor.
- **Automation Engineers** — deploy new flow logic and manage node dependencies via conversation.
- **DevOps Teams** — check system diagnostics and runtime settings across multiple Node-RED instances.


## Available Tools
- **add_flow**: Add a new flow to the configuration
- **delete_flow**: Delete an individual flow
- **get_diagnostics**: js, and memory usage.

Get Node-RED system diagnostics
- **get_flow**: Get an individual flow (tab) configuration
- **get_flows**: Get active flow configuration
- **get_nodes**: Get list of installed nodes
- **install_node**: Install a new node module
- **remove_node**: Remove a node module
- **set_flows**: Set active flow configuration
- **get_settings**: Get Node-RED runtime settings
- **update_flow**: Update an individual flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Node-RED** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active flows in my Node-RED instance."

**🤖 AI Agent:**
> I've retrieved your flows. You have 3 main tabs: 'Home Automation' (ID: f123), 'Data Logger' (ID: f456), and 'Alerts' (ID: f789). Would you like to inspect a specific one?

---

**👤 You:**
> "Check the system diagnostics and memory usage."

**🤖 AI Agent:**
> Diagnostics report: Node.js v18.16.0, OS: Linux. Memory usage is currently at 150MB of 512MB allocated. The system is healthy.

---

**👤 You:**
> "Install the 'node-red-node-email' module."

**🤖 AI Agent:**
> Starting installation of 'node-red-node-email'... The module has been successfully installed and is now available in your palette.


## Installation & Usage

To install and use the **Node-RED** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/node-red](https://vinkius.com/mcp/node-red)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
