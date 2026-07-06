# Woodpecker CI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woodpecker-ci)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage your Woodpecker CI instance — control pipelines, monitor agents, and configure repositories directly from your AI agent.

## Description
Connect your **Woodpecker CI** server to any AI agent to automate your continuous integration and deployment workflows through natural language.

### What you can do

- **Pipeline Control** — List, trigger, restart, or cancel pipelines for any repository to keep your builds moving.
- **Agent Monitoring** — View all connected agents, check their health metrics, and manage task assignments in real-time.
- **Repository Management** — Activate new repositories, update settings, and repair webhooks without leaving your chat interface.
- **Secret & Config Management** — Securely handle global, organization, or repository-level secrets and inspect pipeline configurations.
- **System Insights** — Retrieve server version, health status, and performance metrics to ensure your CI infrastructure is running smoothly.

### How it works

1. Subscribe to this server
2. Provide your Woodpecker Server URL and Personal Access Token
3. Start orchestrating your DevOps workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Monitor build agents and troubleshoot failing pipelines using simple queries.
- **Software Developers** — Trigger builds and check pipeline status directly from the code editor.
- **SREs & System Admins** — Keep an eye on CI infrastructure health and manage secrets across the organization.


## Available Tools (34)
- **cancel_pipeline**: Cancel a running pipeline
- **chown_repo**: Change repository owner to the current user
- **create_agent**: Create a new Woodpecker agent
- **create_global_secret**: Create a global secret
- **create_repo_secret**: Create a repository secret
- **delete_agent**: Delete an agent
- **delete_pipeline**: Delete a pipeline
- **delete_repo**: Deactivate/delete a repository
- **get_agent**: Get details of a specific agent
- **get_healthz**: Server health check
- **get_metrics**: Prometheus metrics (requires WOODPECKER_PROMETHEUS_AUTH_TOKEN if configured)
- **get_org_permissions**: Get user permissions for an organization
- **get_pipeline_config**: Get the configuration files used for a pipeline
- **get_pipeline**: Get details of a specific pipeline
- **get_repo**: Get repository details
- **get_user**: Get the currently authenticated user
- **get_version**: Get server version information
- **list_agent_tasks**: List tasks currently assigned to an agent
- **list_agents**: List all Woodpecker agents
- **list_global_secrets**: List global secrets (Admin only)
- **list_org_agents**: List agents scoped to an organization
- **list_org_secrets**: List organization-level secrets
- **list_orgs**: List all organizations
- **list_pipelines**: List pipelines for a repository
- **list_repo_secrets**: List repository-level secrets
- **list_repos**: List all repositories on the server
- **list_users**: List all users (Admin only)
- **lookup_repo**: Lookup a repository by its full name (slug)
- **repair_repo**: Repair repository webhooks
- **restart_pipeline**: Restart a pipeline
- **trigger_pipeline**: Trigger a manual pipeline
- **update_agent**: Update an existing agent
- **update_repo**: Update repository settings
- **activate_repo**: Activate a repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Woodpecker CI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Woodpecker agents and show their current status."

**🤖 AI Agent:**
> I've retrieved the agent list. You have 3 agents: 'docker-runner-01' (Online), 'k8s-agent-alpha' (Online), and 'legacy-local' (Offline). Would you like to see the tasks assigned to 'docker-runner-01'?

---

**👤 You:**
> "Find the repository 'vinkius/mcp-server' and trigger a new pipeline."

**🤖 AI Agent:**
> Found it (ID: 42). I have triggered a new pipeline for 'vinkius/mcp-server'. The new pipeline is #154. You can monitor its progress or I can notify you when it finishes.

---

**👤 You:**
> "Show me the last 5 pipelines for repository ID 42."

**🤖 AI Agent:**
> Here are the 5 most recent pipelines for repo 42: #153 (Success), #152 (Failure), #151 (Success), #150 (Success), and #149 (Cancelled). Pipeline #152 failed at the 'test' step. Would you like to see the config for that build?


## ❓ FAQ

**Q: Can I trigger a new pipeline build for a specific repository?**
Yes. Use the `trigger_pipeline` tool by providing the repository ID. You can also specify a branch or commit if needed to start a new execution immediately.

**Q: How do I check if my build agents are online and healthy?**
You can use `list_agents` to see all connected agents and their status. For more detail on a specific agent, use `get_agent` or `list_agent_tasks` to see what it's currently working on.

**Q: Is it possible to manage environment secrets through this agent?**
Yes, the server includes tools like `create_repo_secret` and `list_repo_secrets` to manage sensitive variables at the repository level, as well as global and organization-level secret tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woodpecker-ci](https://vinkius.com/mcp/woodpecker-ci)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Woodpecker CI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `woodpecker-ci` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Woodpecker CI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woodpecker-ci": {
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
