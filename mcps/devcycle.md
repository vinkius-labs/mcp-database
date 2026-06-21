# DevCycle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devcycle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/devcycle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/devcycle-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage feature flags, monitor environments, and track variations via the DevCycle API.

## Description
Integrate **DevCycle**, the modern feature flag and experimentation platform, directly into your AI workflow. Manage your feature flags across projects, monitor staging and production environments, and audit targeting rules and variations using natural language.

### What you can do

- **Feature Flag Management** — List, search, and retrieve detailed configuration for all your feature flags.
- **Environment Oversight** — Monitor project environments, retrieve SDK keys, and track deployment statuses.
- **Variable & Variation Tracking** — List all defined variables and their variations to ensure technical consistency.
- **Operational Control** — Update feature flag statuses (active/archived) directly via chat.

### How it works

1. Connect the DevCycle integration to your AI assistant.
2. Authorize using your DevCycle Management API Client ID and Client Secret.
3. Accelerate your software delivery and experimentation through intuitive conversation.

### Who is this for?

- **Software Engineers** — Quickly check flag configurations and SDK keys directly from the IDE or chat.
- **Product Managers** — Monitor feature rollout status and targeting rules during planning.
- **DevOps & SREs** — Audit environment settings and flag statuses during incident response.


## Available Tools
- **get_environment_sdk_keys**: List SDK keys for all environments in a project
- **get_feature_flag_details**: Get full configuration and targeting rules for a specific feature flag
- **get_project_details**: Get detailed information for a specific DevCycle project
- **list_active_flags**: Identify feature flags that are currently active
- **list_project_environments**: List all environments (e.g. Production, Staging) for a project
- **list_devcycle_projects**: List all projects in your DevCycle account
- **list_feature_variables**: List all variables defined in a project
- **list_feature_flags**: g. release, ops), and current statuses.

List all feature flags within a specific project
- **search_feature_flags**: Search for feature flags in a project by keyword
- **update_feature_flag_status**: Update the status (e.g. active, archived) of a feature flag


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DevCycle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all feature flags in the project 'Main-App'."

**🤖 AI Agent:**
> I've found 12 feature flags in 'Main-App', including 'New-Dashboard-UI' (Active) and 'Legacy-Search' (Archived). Would you like to see the targeting rules for the dashboard UI flag?

---

**👤 You:**
> "Show me the configuration for the 'Beta-Feature' flag."

**🤖 AI Agent:**
> The 'Beta-Feature' flag has 2 variations: 'Control' (False) and 'Treatment' (True). It is currently targeting 10% of users in the 'Production' environment. Should I list the specific user IDs included in this rollout?

---

**👤 You:**
> "What are the SDK keys for our 'Production' environment?"

**🤖 AI Agent:**
> For the 'Production' environment, I've retrieved the following keys: Mobile SDK Key (mob_prod_...), Client SDK Key (client_prod_...), and Server SDK Key (server_prod_...). Would you like me to copy the server key for you?


## Installation & Usage

To install and use the **DevCycle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devcycle](https://vinkius.com/mcp/devcycle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
