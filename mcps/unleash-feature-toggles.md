# Unleash (Feature Toggles) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unleash-feature-toggles)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage feature flags, strategies, and environments via Unleash — evaluate toggles, list projects, and monitor metrics directly from your AI agent.

## Description
Connect your **Unleash** instance to any AI agent and gain full control over your feature management lifecycle through natural conversation.

### What you can do

- **Feature Evaluation** — Fetch all feature flags and strategies for server-side evaluation or evaluate specific flags for client-side contexts using User IDs and properties.
- **Project & Environment Audit** — List all Unleash projects, environments, and segments to understand your infrastructure layout.
- **Flag Management** — Inspect all feature flags within specific projects to verify rollout statuses and strategy configurations.
- **Metrics & Registration** — Report SDK usage metrics and register new client or frontend instances directly through the agent.
- **User Management** — Retrieve lists of users and segments to verify targeting rules and access.

### How it works

1. Subscribe to this server
2. Enter your Unleash API URL and API Token (Admin, Client, or Frontend depending on your needs)
3. Start managing your feature rollouts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly audit environments and segments without navigating the Unleash UI
- **Product Managers** — check the status of feature toggles and rollout strategies across different projects
- **Software Engineers** — verify flag evaluations and context properties directly from the code editor


## Available Tools
- **list_environments**: Fetches all environments configured in Unleash.

List all Unleash environments
- **list_project_features**: Fetches features for a given project ID.

List all feature flags in a specific project
- **list_projects**: Fetches all projects configured in Unleash.

List all Unleash projects
- **list_segments**: Fetches all segments configured in Unleash.

List all Unleash segments
- **list_users**: Fetches all users configured in Unleash.

List all Unleash users
- **get_client_features**: Fetch all feature flags and strategies for server-side evaluation
- **report_client_metrics**: Report flag usage metrics from a backend SDK
- **register_client**: Register a new backend SDK instance
- **get_frontend_features**: Optionally provide context like userId or properties.

Fetch enabled feature flags for a specific Unleash Context
- **report_frontend_metrics**: Report flag usage metrics from a frontend SDK
- **register_frontend**: Register a new frontend SDK instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unleash (Feature Toggles)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Unleash projects and their descriptions."

**🤖 AI Agent:**
> I've retrieved the projects. You have 3 projects: 'Default' (Main project), 'Mobile-App' (Flags for iOS/Android), and 'Beta-Testing' (Experimental features).

---

**👤 You:**
> "What feature flags are enabled for user 'user_88' in the frontend?"

**🤖 AI Agent:**
> Evaluating flags for 'user_88'... The following flags are enabled: 'new-dashboard-v2', 'dark-mode-beta', and 'premium-checkout'. Flags like 'experimental-chat' remain disabled for this user context.

---

**👤 You:**
> "Show me all feature flags in the 'Mobile-App' project."

**🤖 AI Agent:**
> In the 'Mobile-App' project, I found 4 flags: 'biometric-login' (Enabled), 'offline-mode' (Disabled), 'push-notifications-v3' (Enabled), and 'legacy-sync' (Disabled).


## ❓ FAQ

**Q: Can I evaluate feature flags for a specific user ID?**
Yes. Use the `get_frontend_features` tool and provide the `userId`. The agent will return the enabled flags based on the Unleash context for that specific user.

**Q: How do I see all feature flags associated with a specific project?**
You can use the `list_project_features` tool by providing the `projectId`. This will list all toggles, their types, and current statuses within that project.

**Q: Does this server support listing segments and environments?**
Yes, the server includes `list_segments` and `list_environments` tools, allowing you to audit your Unleash configuration and targeting rules easily.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unleash-feature-toggles](https://vinkius.com/mcp/unleash-feature-toggles)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unleash (Feature Toggles)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unleash-feature-toggles` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unleash (Feature Toggles)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unleash-feature-toggles": {
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
