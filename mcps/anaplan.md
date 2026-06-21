# Anaplan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anaplan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Anaplan workspaces, models, and data actions (imports, exports, processes) directly via AI.

## Description
Connect your **Anaplan** account to your AI agent to automate financial planning, supply chain, and sales operations. This MCP server allows you to discover workspaces and models, and trigger complex data integration tasks using natural language.

### What you can do

- **Workspace & Model Discovery** — List all available workspaces and models to navigate your planning environment.
- **Execute Data Actions** — Trigger and monitor imports, exports, and processes (groups of actions) to move data in and out of Anaplan.
- **Task Monitoring** — Real-time tracking of asynchronous task statuses to ensure your data integrations complete successfully.
- **File Management** — List files within your models to keep track of historical imports and exports.

### How it works

1. Subscribe to this server
2. Provide your Anaplan Auth Token
3. Start managing your Anaplan environment directly through your AI chat interface.

### Who is this for?

- **FP&A Analysts** — Automate the triggering of planning processes and exports without manual intervention.
- **Supply Chain Managers** — Quickly run data imports for inventory updates via chat.
- **Operations Teams** — Monitor the status of long-running data syncs directly from your workspace.


## Available Tools
- **get_task_status**: Get status of a running task
- **list_exports**: List export actions for a model
- **list_files**: List files in a model (exports/imports)
- **list_imports**: List import actions for a model
- **list_models**: List Anaplan models. Optionally filter by workspaceId
- **list_processes**: List processes for a model
- **list_workspaces**: List available Anaplan workspaces
- **run_export**: Run an Anaplan export action
- **run_import**: Run an Anaplan import action
- **run_process**: Run an Anaplan process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anaplan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Anaplan workspaces and models."

**🤖 AI Agent:**
> I've retrieved your Anaplan environment. You have 2 workspaces: 'Finance_Production' (ID: abc...) and 'Supply_Chain_Test' (ID: def...). Within 'Finance_Production', there are 3 models available.

---

**👤 You:**
> "Run the 'Monthly Actuals' import in the Finance workspace."

**🤖 AI Agent:**
> I've started the 'Monthly Actuals' import task (ID: task_123). I will monitor the status for you. Currently, it is 'IN_PROGRESS'.

---

**👤 You:**
> "What's the status of the process task 'p_456'?"

**🤖 AI Agent:**
> The process task 'p_456' has completed successfully. All 3 sub-actions within the process were finished without errors.


## ❓ FAQ

**Q: How do I find my Workspace and Model IDs?**
You can use the `list_workspaces` and `list_models` tools provided by this server. They will return a list of all accessible environments along with their unique IDs.

**Q: Are actions in Anaplan synchronous or asynchronous?**
Most data actions (imports, exports, processes) are asynchronous. When you run them, they return a Task ID. You should then use `get_task_status` to monitor the progress until it reaches a 'COMPLETE' state.

**Q: Can I trigger an Anaplan process that contains multiple actions?**
Yes, use the `run_process` tool. Processes in Anaplan are designed to run a sequence of imports, exports, and other actions in a specific order. You can monitor the entire process using the returned Task ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anaplan](https://vinkius.com/mcp/anaplan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anaplan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `anaplan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anaplan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anaplan": {
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
