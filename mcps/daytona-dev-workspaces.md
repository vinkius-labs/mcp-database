# Daytona (Dev Workspaces) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/daytona-dev-workspaces)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage ephemeral development environments and sandboxes via Daytona — create, start, stop, and resize workspaces directly from your AI agent.

## Description
Connect your **Daytona** account to any AI agent to orchestrate cloud-based development environments through natural language. Daytona provides standardized, ephemeral sandboxes that can be provisioned and managed on demand.

### What you can do

- **Sandbox Orchestration** — List, create, start, stop, and delete sandboxes with specific CPU, memory, and disk configurations.
- **Snapshot Management** — Create and manage snapshots to preserve environment states or activate them for new sandboxes using `create_snapshot` and `activate_snapshot`.
- **API Key Control** — Manage your authentication keys directly, including listing and creating new access tokens via `list_api_keys` and `create_api_key`.
- **Resource Scaling** — Dynamically resize sandbox resources (vCPU, RAM, Disk) to match your workload requirements using `resize_sandbox`.
- **Volume & Storage** — Inspect and manage persistent volumes and snapshots for your dev environments.

### How it works

1. Subscribe to this server
2. Enter your Daytona API Key
3. Start managing your dev infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — Automate the lifecycle of test environments and sandboxes.
- **Software Developers** — Spin up fresh coding environments without leaving the chat or IDE.
- **QA Teams** — Quickly recover sandboxes from error states or fork existing environments for debugging.


## Available Tools (28)
- **create_sandbox**: Create a new Daytona sandbox
- **create_snapshot**: Create a new snapshot
- **deactivate_snapshot**: Deactivate a snapshot
- **delete_api_key**: Delete an API key by name
- **delete_sandbox**: Delete a sandbox
- **delete_snapshot**: Delete a snapshot
- **delete_volume**: Delete a volume
- **fork_sandbox**: Fork an existing sandbox
- **get_api_key**: Get details of a specific API key by name
- **get_current_api_key**: Get details of the currently authenticated API key
- **get_sandbox_preview_url**: Get a signed preview URL for a specific port on a sandbox
- **get_sandbox**: Get details of a specific sandbox
- **get_snapshot**: Get details of a specific snapshot
- **get_volume_by_name**: Get details of a specific volume by name
- **get_volume**: Get details of a specific volume by ID
- **list_api_keys**: List Daytona API keys
- **list_sandboxes_paginated**: List all Daytona sandboxes (paginated)
- **list_sandboxes**: List all Daytona sandboxes
- **list_snapshots**: List all Daytona snapshots
- **list_volumes**: List all Daytona volumes
- **recover_sandbox**: Recover a sandbox from an error state
- **resize_sandbox**: Resize sandbox resources
- **start_sandbox**: Start a stopped sandbox
- **stop_sandbox**: Stop a running sandbox
- **activate_snapshot**: Activate a snapshot
- **archive_sandbox**: Archive a sandbox
- **create_api_key**: Create a new Daytona API key
- **create_volume**: Create a new volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daytona (Dev Workspaces)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Daytona sandboxes."

**🤖 AI Agent:**
> I've retrieved your sandboxes. You have 3 active environments: 'web-app-dev', 'api-testing', and 'database-sandbox'. Would you like details on any of them?

---

**👤 You:**
> "Create a new sandbox with 2 CPUs and 4GB of RAM using the node:20 image."

**🤖 AI Agent:**
> Starting the creation process for a new sandbox with 2 vCPUs, 4GB RAM, and the 'node:20' image. I'll let you know once it's provisioned.

---

**👤 You:**
> "Stop the sandbox named 'dev-environment-1'."

**🤖 AI Agent:**
> Stopping 'dev-environment-1' now. The resources will be released while preserving your data.


## ❓ FAQ

**Q: Can I change the resources of an existing sandbox?**
Yes, you can use the `resize_sandbox` tool to update the CPU, memory, or disk size of a specific sandbox by providing its ID or name.

**Q: How do I create a new environment with a specific Docker image?**
Use the `create_sandbox` tool and provide the `image` parameter with the desired Docker or OCI image name.

**Q: What should I do if a sandbox is in an error state?**
You can use the `recover_sandbox` tool to attempt to restore a sandbox from an error state back to a functional one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daytona-dev-workspaces](https://vinkius.com/mcp/daytona-dev-workspaces)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daytona (Dev Workspaces)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `daytona-dev-workspaces` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daytona (Dev Workspaces)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "daytona-dev-workspaces": {
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
