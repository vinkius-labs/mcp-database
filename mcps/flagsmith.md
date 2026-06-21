# Flagsmith MCP Server

Manage feature flags and remote config via Flagsmith — toggle features, manage identities, and update environment configurations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flagsmith)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **Flagsmith** account to any AI agent to control feature releases and remote configurations through natural conversation.

### What you can do

- **Flag Management** — Retrieve default flag states and remote configuration values for any environment instantly.
- **Identity Control** — Fetch specific flags and traits for user identities or identify new users with custom traits to test personalized experiences.
- **Environment Admin** — Create new environments within projects and fetch full configuration documents for local evaluation modes.
- **Dynamic Updates** — Update flag values (single or batch) and manage segment overrides using the Admin API for rapid iteration.
- **Local Evaluation** — Access the entire environment configuration document for high-performance SDK integrations.

### How it works

1. Subscribe to this server
2. Enter your Flagsmith Environment Key or Admin API Key
3. Start managing your feature lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — check flag states and user traits directly from the code editor to debug feature logic without switching contexts.
- **Product Managers** — toggle features, manage rollouts, and update remote configs without touching the dashboard.
- **DevOps & SREs** — automate environment creation and manage segment overrides through simple natural language commands.


## Available Tools
- **create_environment**: Requires FLAGSMITH_API_KEY.

Create a new environment within a project
- **delete_segment_override**: Requires FLAGSMITH_API_KEY.

Delete a segment override
- **get_environment_document**: Requires FLAGSMITH_ENVIRONMENT_KEY.

Get the entire environment configuration document
- **get_environment_flags**: Requires FLAGSMITH_ENVIRONMENT_KEY.

Get all default flag states for an environment
- **get_identity_flags**: Requires FLAGSMITH_ENVIRONMENT_KEY.

Get flags and traits for a specific user identity
- **identify_user**: Requires FLAGSMITH_ENVIRONMENT_KEY.

Identify user and set traits
- **update_flag_v1**: Requires FLAGSMITH_API_KEY.

Update a flag value (Single change)
- **update_flag_v2**: Requires FLAGSMITH_API_KEY.

Update flags (Batch change)


## Installation & Usage

To install and use the **Flagsmith** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flagsmith](https://vinkius.com/mcp/flagsmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
