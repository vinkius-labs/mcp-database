# Cursor Cloud Agent MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cursor-cloud-agent)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Create and manage Cursor cloud agents — spin up autonomous coding agents, track runs, monitor usage, and manage artifacts from any AI assistant.

## Description
Connect your **Cursor** API key to any AI agent and unlock the full power of Cursor Cloud Agents through natural conversation.

### What you can do

- **Create Agents** — Spin up autonomous coding agents with a prompt, model selection, repository access, and mode configuration (agent or plan)
- **Manage Agents** — List, get details, archive, and restore cloud agents with full lifecycle control
- **Run Agents** — Trigger new runs on existing agents with custom prompts, images, MCP server configurations, and mode overrides
- **Track Runs** — List all runs, get detailed status with duration and git branch info, and cancel long-running runs
- **Monitor Usage** — Get token usage breakdowns including input, output, and cache tokens per agent or per run
- **Discover Artifacts** — List all artifacts (files) produced by an agent's runs with paths and sizes
- **Verify Identity** — Check the authenticated API user with the get_me endpoint

### How it works

1. Subscribe to this server
2. Enter your Cursor API key (create one at Cursor Dashboard → API Keys)
3. Start creating and managing cloud agents from Claude, Cursor, or any MCP-compatible client

Your AI acts as a control plane for Cursor's autonomous coding agents — create agents, trigger runs, monitor progress, and manage the entire agent lifecycle without writing a single line of code.

### Who is this for?

- **Engineering Teams** — automate repetitive coding tasks by spinning up agents that work in your repos
- **DevOps** — orchestrate autonomous code changes, PRs, and reviews across multiple repositories
- **Platform Teams** — monitor agent usage and token consumption for cost optimization
- **Developers** — delegate coding tasks to cloud agents and track results from your AI chat


## Available Tools (12)
- **unarchive_agent**: This operation is idempotent — unarchiving an already-active agent succeeds without error.

Restore an archived Cursor cloud agent. Idempotent operation
- **archive_agent**: The agent is no longer active but can be restored with unarchive_agent. This operation is idempotent — archiving an already-archived agent succeeds without error.

Archive (soft delete) a Cursor cloud agent. Idempotent operation
- **cancel_run**: This is a terminal cancellation — once cancelled, the run cannot be resumed. Use this when a run is taking too long or is no longer needed.

Cancel a running Cursor cloud agent run. Terminal operation
- **create_agent**: The agent receives a prompt (required), can be configured with a model (e.g. gpt-4.1, claude-sonnet-4-20250514, gemini-2.5-pro), optional repository URLs with starting refs, autoCreatePR flag, and mode (agent or plan). Returns the agent object and an initial run object.

Create a new Cursor cloud agent with a prompt and optional repos, model, and mode
- **create_run**: The run receives a prompt (required), optional images, optional MCP servers, and an optional mode override. Returns the run object with status and ID.

Create a new run for an existing Cursor cloud agent
- **get_agent**: Use this to check agent configuration or status.

Get full metadata for a specific Cursor cloud agent
- **get_agent_usage**: Optionally filter by runId to get usage for a specific run.

Get token usage statistics for a Cursor cloud agent
- **get_me**: Use this to verify API key validity and identify the authenticated account.

Get information about the authenticated Cursor API user
- **get_run**: Use this to check if a run completed, see its output, or inspect git branches it created.

Get details and status of a specific Cursor cloud agent run
- **list_agents**: Supports limit (default 20, max 100), cursor for pagination, prUrl to filter by PR, and includeArchived (default true). Returns items array and nextCursor for pagination.

List all Cursor cloud agents with pagination and filtering
- **list_artifacts**: Use this to discover what files the agent created or modified.

List all artifacts produced by a Cursor cloud agent
- **list_runs**: Supports limit and cursor for pagination. Returns items array with run summaries.

List all runs for a specific Cursor cloud agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cursor Cloud Agent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a cloud agent to add a README file to my repository."

**🤖 AI Agent:**
> Creating a cloud agent... Done! Agent `agent-001` has been created with the prompt 'Add a README file to this repository' and is now running. The initial run `run-001` has started — you can check its status with `get_run`. Would you like me to enable autoCreatePR so the agent opens a pull request when it finishes?

---

**👤 You:**
> "List all my cloud agents and show their status."

**🤖 AI Agent:**
> Fetching your agents... Found 3 agents:
1. **README Agent** (`agent-001`) — status: `active`, latest run: `run-005` (completed)
2. **Bug Fixer** (`agent-002`) — status: `active`, latest run: `run-008` (running)
3. **Doc Generator** (`agent-003`) — status: `archived`

Would you like me to get details on a specific agent or check the status of the running `run-008`?

---

**👤 You:**
> "Get the status and result of run run-008 on agent agent-002."

**🤖 AI Agent:**
> Checking run `run-008` on agent `agent-002`... Status: `completed`. Duration: 45,000 ms (45s). The agent successfully fixed the bug and created a commit on branch `bugfix/issue-42`. Result summary: 'Fixed null pointer exception in the auth middleware by adding a null check before accessing the user object.' A pull request was automatically created at https://github.com/example/repo/pull/42. Would you like me to check the token usage for this run?


## ❓ FAQ

**Q: How do I get my Cursor API key?**
Go to the **Cursor Dashboard → API Keys** section to create or manage your API key. The key starts with `crsr_` and can be either a user API key or a service account API key. Copy it and paste it into the API key field in the setup wizard. The key is sent as a Bearer token in the Authorization header for all API requests.

**Q: What are Cursor cloud agents?**
Cloud agents are autonomous coding agents that run in Cursor's managed environment. You give them a prompt describing what you want (e.g. 'Add a README file to this repo'), connect one or more repositories, and the agent works autonomously — reading code, making changes, and optionally creating pull requests. You can track run status, view results, and manage the agent lifecycle through the API.

**Q: Can cloud agents automatically create pull requests?**
Yes! When creating an agent, set the `autoCreatePR` flag to `true` and the agent will automatically create a pull request when it finishes its work. You can also filter agents by PR URL using the `pr_url` parameter in the `list_agents` tool to find agents associated with a specific PR.

**Q: Which models are supported by cloud agents?**
Cursor cloud agents support multiple AI models including **gpt-4.1**, **claude-sonnet-4-20250514**, and **gemini-2.5-pro**. You can specify the model when creating an agent using the `model_id` parameter. If no model is specified, Cursor uses its default model. The model determines which AI processes your agent's prompts and generates code changes.

**Q: How do I track the status of a run?**
Use the `get_run` tool with the agent ID and run ID to get the full status including the current state (running, completed, cancelled), duration in milliseconds, the result output, and git branch information. You can also use `list_runs` to see all runs for an agent. To stop a long-running run, use `cancel_run` — this is a terminal operation that cannot be undone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cursor-cloud-agent](https://vinkius.com/mcp/cursor-cloud-agent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cursor Cloud Agent** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cursor-cloud-agent` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cursor Cloud Agent** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cursor-cloud-agent": {
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
