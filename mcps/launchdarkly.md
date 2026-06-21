# LaunchDarkly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/launchdarkly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/launchdarkly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/launchdarkly-mcp)
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


## Available Tools
- **get_environment**: Get details regarding an environment
- **get_feature_flag**: Get in-depth specifics for a feature flag
- **get_metric**: Get details for a specific metric
- **get_project**: Get details for a specific project
- **list_audit_logs**: Retrieve audit log entries for the account
- **list_environments**: g. Test, Production).

Retrieve all environments within a project
- **list_feature_flags**: Retrieve feature flags within a project
- **list_metrics**: Retrieve experimentation metrics within a project
- **list_projects**: Retrieve a list of LaunchDarkly projects


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


## Installation & Usage

To install and use the **LaunchDarkly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/launchdarkly](https://vinkius.com/mcp/launchdarkly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
