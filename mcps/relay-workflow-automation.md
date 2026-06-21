# Relay Workflow Automation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/relay-workflow-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

List, run, and manage workflow automations via Relay API.

## Description
Connect **Relay** to any AI agent and automate your business workflows -- list available workflows, trigger executions with dynamic inputs, monitor run statuses, and cancel active runs through natural conversation.

### What you can do
- **Workflow Discovery** -- List and inspect all configured workflows in your account
- **Trigger Execution** -- Start workflows with custom input variables
- **Run Monitoring** -- Check progress and results of active and completed runs
- **Run Management** -- Cancel in-progress workflows when needed

### How it works
1. Subscribe to this server
2. Enter your Relay API Key from Dashboard Settings
3. Start managing automations from Claude, Cursor, or any MCP-compatible client

Relay is a no-code workflow automation platform used by teams to connect apps, automate processes, and reduce manual work.

### Who is this for?
- **Operations Teams** -- Trigger and monitor workflows without opening the Relay dashboard
- **Support Agents** -- Run customer-specific workflows with dynamic inputs
- **Developers** -- Integrate Relay automations into AI agent workflows and apps


## Available Tools
- **list_workflows**: Use this to discover available automations before running them.

List all workflows in your Relay account
- **get_run_status**: Get the current status of a workflow run
- **get_workflow**: Get details of a specific workflow
- **list_runs**: List recent workflow runs
- **run_workflow**: Provide a JSON object of input variables required by the workflow.

Trigger a workflow execution with optional inputs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relay Workflow Automation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my workflows."

**🤖 AI Agent:**
> Found 4 workflows: 1. Customer Onboarding. 2. Invoice Processing. 3. Lead Qualification. 4. Weekly Report.

---

**👤 You:**
> "Run the 'Customer Onboarding' workflow with inputs {email: 'john@example.com', name: 'John Doe'}."

**🤖 AI Agent:**
> Workflow run started! Run ID: run_abc123. Status: running.

---

**👤 You:**
> "Check the status of run run_abc123."

**🤖 AI Agent:**
> Run run_abc123: Status: completed. Output: Account created successfully.


## ❓ FAQ

**Q: How do I get my Relay API Key?**
Log in to your Relay account, navigate to Settings > API Keys, and generate a new key.

**Q: Can I pass inputs to a workflow?**
Yes! Use the run_workflow action with a JSON object of input variables that match your workflow's input schema.

**Q: Can I cancel an active workflow run?**
Yes! Use the cancel_run action with the run ID. This only works on runs that are currently in progress.

**Q: Can I view the required inputs for a specific workflow?**
Yes! Use the get_workflow action to see its required input schema before running it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/relay-workflow-automation](https://vinkius.com/mcp/relay-workflow-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relay Workflow Automation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `relay-workflow-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relay Workflow Automation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relay-workflow-automation": {
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
