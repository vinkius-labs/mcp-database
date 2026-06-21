# Flagsmith MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flagsmith)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flagsmith-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flagsmith-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage feature flags and remote config via Flagsmith — toggle features, manage identities, and update environment configurations directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flagsmith** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get all default flag states for my current environment."

**🤖 AI Agent:**
> I've retrieved the flags for your environment. There are 12 active flags, including 'new_onboarding_flow' (Enabled) and 'beta_search_algorithm' (Disabled). Would you like the details of any specific flag?

---

**👤 You:**
> "Identify user 'user_99' and set their 'subscription' trait to 'premium'."

**🤖 AI Agent:**
> User 'user_99' has been identified and their traits updated. Based on the 'premium' subscription trait, they now have access to the 'advanced_analytics' and 'priority_support' flags.

---

**👤 You:**
> "Update the flag value for environment 'ser_key_123' to enable the 'maintenance_mode' feature."

**🤖 AI Agent:**
> I have successfully updated the flag. The 'maintenance_mode' feature is now enabled for environment 'ser_key_123'.


## Installation & Usage

To install and use the **Flagsmith** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flagsmith](https://vinkius.com/mcp/flagsmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
