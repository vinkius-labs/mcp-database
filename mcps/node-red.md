# Node-RED MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/node-red)
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


## ❓ FAQ

**Q: Can I install new nodes from npm using this server?**
Yes. Use the `install_node` tool and provide the npm module name. The server will trigger the installation in your Node-RED instance.

**Q: How can I check if my Node-RED server is running out of memory?**
You can run the `get_diagnostics` tool. It returns real-time system metrics including memory usage, Node.js version, and OS information.

**Q: Is it possible to delete a specific flow tab?**
Yes, by using the `delete_flow` tool with the specific Flow ID. Be careful, as this action will permanently remove that flow configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/node-red](https://vinkius.com/mcp/node-red)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Node-RED** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `node-red` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Node-RED** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "node-red": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
