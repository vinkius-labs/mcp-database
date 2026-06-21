# DevCycle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devcycle)
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


## ❓ FAQ

**Q: How do I get DevCycle API credentials?**
Log in to your DevCycle dashboard, navigate to **Settings > Organization > API Management**, and create a new Client ID and Client Secret.

**Q: Can the agent toggle feature flags?**
Yes, you can use the update_feature_flag_status tool to set a flag to 'active' or 'archived' directly from the agent.

**Q: Does the integration show SDK keys?**
Yes, the get_environment_sdk_keys tool allows the agent to retrieve the specific identifiers needed for your web, mobile, or server-side SDKs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devcycle](https://vinkius.com/mcp/devcycle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DevCycle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `devcycle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DevCycle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devcycle": {
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
