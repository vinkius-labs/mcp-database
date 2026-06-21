# Daytona (Dev Workspaces) MCP Server

Manage ephemeral development environments and sandboxes via Daytona — create, start, stop, and resize workspaces directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/daytona-dev-workspaces)

## Overview
**Category:** developer-tools
**Tools Count:** 28

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


## Available Tools
- **activate_snapshot**: Activate a snapshot
- **archive_sandbox**: Archive a sandbox
- **create_api_key**: Create a new Daytona API key
- **create_sandbox**: Create a new Daytona sandbox
- **create_snapshot**: Create a new snapshot
- **create_volume**: Create a new volume
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


## Installation & Usage

To install and use the **Daytona (Dev Workspaces)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daytona-dev-workspaces](https://vinkius.com/mcp/daytona-dev-workspaces)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
