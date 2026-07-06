# LaunchDarkly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/launchdarkly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage LaunchDarkly feature flags, environments, assignments and deployments smoothly through conversational AI.

## Description
Connect your **LaunchDarkly** platform to any AI agent to monitor experiments and toggle feature flags without breaking your flow.

### What you can do

- **Flag Management:** List existing configurations and inspect deployment flags.
- **Environment Variables:** Map contexts directly from your active workspaces.
- **Experiments:** Safely inspect tracking parameters and current user engagement strategies.

### How it works

1. Install this MCP Server locally
2. Supply your LaunchDarkly API token key
3. Start fetching and triggering project deployments on the command line

### Who is this for?

- **DevOps Engineers** — enable release monitoring without dashboards
- **Product Teams** — view A/B testing flag statuses immediately
- **Fullstack Devs** — check if your newly pushed feature flag is live


## Available Tools (9)
- **get_feature_flag**: Get in-depth specifics for a feature flag
- **get_metric**: Get details for a specific metric
- **get_project**: Get details for a specific project
- **list_audit_logs**: Retrieve audit log entries for the account
- **list_environments**: g. Test, Production).

Retrieve all environments within a project
- **list_feature_flags**: Retrieve feature flags within a project
- **list_metrics**: Retrieve experimentation metrics within a project
- **list_projects**: Retrieve a list of LaunchDarkly projects
- **get_environment**: Get details regarding an environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LaunchDarkly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the newly implemented dark mode feature flag is switched on in Production."

**🤖 AI Agent:**
> Searching the Production workspace... The UI Dark Mode feature toggle is currently set to ON targeting 50% of the active user base.

---

**👤 You:**
> "Turn off the experimental flag targeting our staging environment immediately."

**🤖 AI Agent:**
> Executing shutdown on experimental flag. The flag has been returned to its OFF (kill switch) state in Staging.

---

**👤 You:**
> "List all active environments linked to our main workspace project."

**🤖 AI Agent:**
> Scanning project environments... I found 3 connected clusters: Staging, Production, and Beta Testing Node.


## ❓ FAQ

**Q: How do I authenticate?**
Generate a valid API access token inside your LaunchDarkly Authorization Settings and attach it.

**Q: Can I toggle flags in Production directly?**
Yes! Due to the direct integration, whatever environments the API token has rights to, the agent can configure.

**Q: Do I need to re-sync manual changes?**
No, the agent fetches live configuration directly from the provider in real-time each run.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/launchdarkly](https://vinkius.com/mcp/launchdarkly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LaunchDarkly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `launchdarkly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LaunchDarkly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "launchdarkly": {
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
