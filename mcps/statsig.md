# Statsig MCP Server

Manage feature flags, dynamic configs, and experiments. Evaluate gates and log events directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/statsig)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **Statsig** project to any AI agent to manage feature rollouts and product experiments through natural conversation.

### What you can do

- **Feature Gates** — Evaluate if a feature is enabled for a specific user or list all project gates
- **Dynamic Configs** — Fetch JSON configurations and experiments to control app behavior without code changes
- **Event Logging** — Log custom events for real-time analytics and metric calculation
- **Gate Management** — Create, update, or delete feature gates directly via the Console API
- **Layer Inspection** — Evaluate layers and retrieve parameter values for specific users

### How it works

1. Subscribe to this server
2. Enter your Statsig Server Secret Key (for evaluation) and Console API Key (for management)
3. Start managing your product experiments from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — check gate statuses and create new feature flags without leaving the chat
- **Developers** — verify evaluation logic and log test events directly from the IDE
- **Data Scientists** — inspect experiment configurations and verify metric logging


## Available Tools
- **check_gate**: Requires STATSIG_SERVER_SECRET_KEY.

Evaluates one or more feature gates for a user
- **create_dynamic_config**: Requires STATSIG_CONSOLE_API_KEY.

Create a new dynamic config
- **create_gate**: Requires STATSIG_CONSOLE_API_KEY.

Create a new feature gate
- **delete_gate**: Requires STATSIG_CONSOLE_API_KEY.

Delete a feature gate
- **get_config**: Requires STATSIG_SERVER_SECRET_KEY.

Fetches configuration values for a dynamic config or experiment
- **get_dynamic_config**: Requires STATSIG_CONSOLE_API_KEY.

Read a specific dynamic config
- **get_gate**: Requires STATSIG_CONSOLE_API_KEY.

Read a specific feature gate
- **get_layer**: Requires STATSIG_SERVER_SECRET_KEY.

Fetches parameter values from a layer
- **list_dynamic_configs**: Requires STATSIG_CONSOLE_API_KEY.

List all dynamic configs in the project
- **list_gates**: Requires STATSIG_CONSOLE_API_KEY.

List all feature gates in the project
- **log_event**: Requires STATSIG_SERVER_SECRET_KEY.

Logs custom events for analytics and metric calculation
- **update_gate**: Requires STATSIG_CONSOLE_API_KEY.

Update an existing feature gate


## Installation & Usage

To install and use the **Statsig** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statsig](https://vinkius.com/mcp/statsig)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
