# Langflow (Visual Multi-agent Orchestrator) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langflow-visual-multi-agent-orchestrator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Orchestrate multi-agent AI workflows visually — execute flows, manage projects, and trigger webhooks directly from any AI agent.

## Description
Connect your **Langflow** instance to any AI agent and take full control of your multi-agent orchestration through natural conversation.

### What you can do

- **Flow Execution** — Run specific flows by ID or name using `run_flow`, supporting both chat and text input types.
- **Workflow Management** — Execute complex background jobs with `run_workflow` or use the OpenAI-compatible `create_response` endpoint.
- **Project Organization** — List, create, and manage projects (folders) to keep your agentic workflows structured via `list_projects`.
- **Flow Lifecycle** — Query, update, or delete existing flows directly from your conversation to iterate on agent logic in real-time.
- **External Triggers** — Start flow runs in response to external events using the `trigger_webhook` tool.

### How it works

1. Subscribe to this server
2. Enter your Langflow Base URL and API Key
3. Start orchestrating complex AI agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — rapidly test and trigger complex RAG or multi-agent flows without leaving the terminal or code editor.
- **Product Teams** — monitor and manage flow versions and project folders through simple natural language queries.
- **DevOps & Automation Leads** — integrate visual AI logic into broader systems by triggering webhooks and background workflows.


## Available Tools
- **create_flow**: Create a new flow
- **create_project**: Create a new project
- **create_response**: Uses flow_id as the model.

OpenAI compatible responses endpoint
- **delete_file_v2**: Delete a file (v2)
- **delete_flow**: Delete a flow
- **delete_project**: Delete a project
- **get_file_v2**: Download a file (v2)
- **get_flow**: Get a specific flow by ID
- **get_logs**: Retrieve recent logs
- **get_monitor_messages**: Retrieve chat history
- **get_monitor_traces**: Retrieve execution traces and span trees
- **get_monitor_transactions**: Retrieve component interaction logs
- **get_project**: Get project details
- **list_files_v1**: List files for a specific flow (v1)
- **list_files_v2**: List user files (v2)
- **list_flows**: List all flows
- **list_projects**: List all projects
- **list_users**: List all users (requires superuser)
- **run_flow**: Supports chat or text inputs.

Execute a Langflow flow
- **run_workflow**: Run a workflow (v2 API)
- **trigger_webhook**: Trigger a Langflow webhook
- **update_flow**: Update an existing flow
- **update_project**: Update project info
- **whoami**: Get current authenticated user info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Langflow (Visual Multi-agent Orchestrator)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available flows in Langflow."

**🤖 AI Agent:**
> I've retrieved your flows. You have 3 active flows: 'Customer Support Agent' (ID: flow-123), 'Data Extraction Pipeline' (ID: flow-456), and 'Market Analyzer' (ID: flow-789).

---

**👤 You:**
> "Run the 'Market Analyzer' flow with the input 'Analyze NVIDIA stock performance'."

**🤖 AI Agent:**
> Executing 'Market Analyzer'... The flow has completed. The analysis suggests a bullish trend for NVIDIA based on recent quarterly results and AI demand.

---

**👤 You:**
> "Show me all my project folders."

**🤖 AI Agent:**
> I found 2 projects: 'Production Agents' (ID: proj-001) and 'Experimental Lab' (ID: proj-002).


## ❓ FAQ

**Q: Can I run a flow using its name instead of a long UUID?**
Yes! The `run_flow` tool accepts either the Flow ID or the Flow Name in the `flow_id` parameter, making it easy to trigger specific logic by name.

**Q: How do I see all the available projects and folders in my Langflow instance?**
Use the `list_projects` tool. It will return a list of all projects (folders) which help organize your flows and components.

**Q: Is it possible to trigger a flow from an external webhook payload?**
Absolutely. Use the `trigger_webhook` tool by providing the `flow_id` and the `data` JSON payload you want to send to the flow's entry point.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langflow-visual-multi-agent-orchestrator](https://vinkius.com/mcp/langflow-visual-multi-agent-orchestrator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Langflow (Visual Multi-agent Orchestrator)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `langflow-visual-multi-agent-orchestrator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Langflow (Visual Multi-agent Orchestrator)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "langflow-visual-multi-agent-orchestrator": {
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
