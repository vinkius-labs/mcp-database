# Buildkite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buildkite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Automate CI/CD pipelines via Buildkite — manage builds, agents, and deployments directly from any AI agent.

## Description
Connect your **Buildkite** account to any AI agent and take full control of your CI/CD workflows through natural conversation.

### What you can do

- **Pipelines & Builds** — List active pipelines, trigger new builds, retry failed executions, or cancel stuck pipelines instantly
- **Deep Log Inspection** — Retrieve the exact details of specific builds, examining job lists, statuses, and tracking links
- **Agent Management** — Ping your connected build agents globally and verify their status
- **Organizational Overview** — Monitor your organization's scale, retrieve active pipelines across the entire company, and get recent builds map

### How it works

1. Subscribe to this server
2. Enter your Buildkite API Token and Organization Slug
3. Start managing your CI/CD pipelines from Claude, Cursor, or any MCP-compatible client

No more context-switching to the terminal or web console. Your AI agent becomes your build operation center.

### Who is this for?

- **DevOps & Platform Teams** — orchestrate hybrid CI infrastructure, monitor hanging processes, and cancel stuck builds effortlessly
- **Software Engineers** — trigger ad-hoc test runs on specific feature branches without leaving your IDE
- **Tech Leads** — get a clean summary of the team's build failure rates before merging to production


## Available Tools (11)
- **cancel_build**: Cancel a running build
- **create_build**: Trigger a new build for a pipeline
- **get_access_token_info**: Retrieve information about the current API token
- **get_build**: Get details of a specific build
- **get_pipeline**: Get details of a specific pipeline
- **list_agents**: List all build agents in the organization
- **list_all_builds**: List all builds across the entire organization
- **list_organizations**: List all organizations the token has access to
- **list_pipeline_builds**: List builds for a specific pipeline
- **list_pipelines**: List all pipelines in the organization
- **rebuild**: Rebuild a specific build


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buildkite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What recent builds ran on our production pipeline?"

**🤖 AI Agent:**
> I checked your recent pipeline execution logs. Build #204 passed on the main branch, but Build #205 failed on the frontend-refactor branch. Would you like me to inspect the failed build's logs?

---

**👤 You:**
> "Cancel build #205 because of a wrong commit."

**🤖 AI Agent:**
> Got it. I've sent the cancellation command to Buildkite for Build #205 on the frontend-refactor pipeline. The agent runners have been halted and the state is now marked as cancelled.

---

**👤 You:**
> "Trigger a new build on HEAD of the main branch for our react-app."

**🤖 AI Agent:**
> I've successfully created a new build execution for the react-app pipeline targeting 'HEAD' on the 'main' branch. It's now running. Let me know if you want me to monitor its status.


## ❓ FAQ

**Q: Can my AI agent restart failed builds for a specific branch?**
Yes. Ask the agent to find failed builds across your pipeline by using the list builds tool. Once it locates the specific build number, it can run the rebuild tool instantly, eliminating the need to search through hundreds of logs on the dashboard.

**Q: How can I check the status of my physical runner agents?**
Ask your agent to list all agents connected to the Buildkite organization. It returns their UUIDs, operating systems, and connection state. If a runner hangs offline, your AI can immediately flag it to the Platform team, saving crucial deployment time.

**Q: If a commit is pushed to 'main', can the agent trigger a fresh pipeline deployment?**
Absolutely. You can provide the commit SHA (or simply ask it to target 'HEAD' on the 'main' branch) and ask the agent to create a new build. It will hit the Buildkite trigger endpoint with a message of your choosing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buildkite](https://vinkius.com/mcp/buildkite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buildkite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buildkite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buildkite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buildkite": {
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
