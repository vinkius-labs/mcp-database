# Optimizely MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/optimizely)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage A/B tests and feature flags via Optimizely — list projects, track experiments, and toggle features directly from any AI agent.

## Description
Connect your **Optimizely** account to any AI agent and take full control of your experimentation and feature management workflows through natural conversation.

### What you can do

- **Project Overview** — List all projects and retrieve detailed metadata to maintain a clear view of your workspace.
- **Experiment Management** — List experiments, check current status (running, paused, draft), and retrieve detailed configurations.
- **Feature Flag Tracking** — List feature flags and inspect their definitions across different projects.
- **Audience & Event Auditing** — List defined audiences and conversion events to verify your targeting and tracking setup.
- **Live Controls** — Start or pause experiments directly through the agent to react quickly to results or issues.

### How it works

1. Subscribe to this server
2. Enter your Optimizely Personal Access Token
3. Start managing your experiments from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check the status of an experiment or toggle a feature flag while reviewing product requirements.
- **Growth Engineers** — audit experiment configurations and audience definitions during implementation.
- **Data Scientists** — retrieve experiment metadata and event definitions for analysis tasks.


## Available Tools (10)
- **get_experiment**: Get details for a specific experiment
- **get_feature_flag**: Get details for a specific feature flag
- **get_project**: Get details for a specific project
- **list_audiences**: List defined audiences in a project
- **list_events**: List conversion events in a project
- **list_experiments**: List experiments in a project
- **list_feature_flags**: List feature flags in a project
- **list_projects**: List all Optimizely projects
- **pause_experiment**: Set experiment status to paused
- **start_experiment**: Set experiment status to running


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Optimizely** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Optimizely projects in my account."

**🤖 AI Agent:**
> I've retrieved 4 projects: 'Main Website', 'Mobile App iOS', 'Checkout Flow', and 'New Product Beta'. Which one would you like to explore?

---

**👤 You:**
> "Check the status of all experiments in project 12345."

**🤖 AI Agent:**
> There are 5 experiments in project 12345. 2 are currently running ('Hero Banner v2', 'Free Shipping Prompt'), 2 are paused, and 1 is in draft mode.

---

**👤 You:**
> "Pause experiment 67890 in project 12345."

**🤖 AI Agent:**
> Experiment 67890 ('Hero Banner v2') has been successfully paused.


## ❓ FAQ

**Q: Where do I find my Personal Access Token?**
In Optimizely, go to **Profile Settings** > **API Access** and generate a new Personal Access Token. Ensure it has the necessary permissions for the projects you want to manage.

**Q: Can I start an experiment that is in draft mode?**
Yes, using the `start_experiment` tool will attempt to set the status to 'running'. However, Optimizely requires the experiment to be valid and fully configured before it can transition from draft to running.

**Q: How do I find my Project ID?**
You can use the `list_projects` tool to see all projects associated with your account along with their IDs. You can also find it in the URL when viewing a project in the Optimizely dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/optimizely](https://vinkius.com/mcp/optimizely)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Optimizely** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `optimizely` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Optimizely** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "optimizely": {
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
