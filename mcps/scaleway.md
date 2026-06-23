# Scaleway MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scaleway)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: How do I see my servers in a specific region like Paris?**
Use the `list_instances` tool and provide the zone parameter (e.g., 'fr-par-1'). The agent will return a list of all instances currently provisioned in that specific Scaleway zone.

**Q: Can I reboot or shut down a server using this integration?**
Yes! The `perform_instance_action` tool allows you to send 'poweron', 'poweroff', 'reboot', or 'terminate' commands to any specific server ID within a zone.

**Q: What information is needed to create a new instance?**
To use `create_instance`, you need to provide the zone, a name for the server, the commercial type (e.g., 'DEV1-S'), and the image ID or label you wish to deploy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scaleway](https://vinkius.com/mcp/scaleway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scaleway** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scaleway` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scaleway** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scaleway": {
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
