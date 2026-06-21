# Lindy (Autonomous AI Employees) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lindy-autonomous-ai-employees)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Manage autonomous AI employees via Lindy — trigger task runs, monitor reasoning logs, and audit app integrations.

## Description
Connect your **Lindy.ai** account to any AI agent and take full control of your autonomous AI workforce and automated business processes through natural conversation.

### What you can do

- **Lindy Orchestration** — List all custom autonomous assistants (Lindies) built in your workspace and retrieve their core configurations and prompt instructions directly from your agent
- **Task Execution** — Trigger specific Lindies to start asynchronous task runs using dynamic JSON payloads to automate complex business workflows
- **Reasoning Audit** — Dump literal LLM reasoning logs for specific run loops to understand how your autonomous agents are making decisions and identifying steps
- **Run Monitoring** — Track the state of active executions and manage lifecycle controls, including the ability to cancel runs stuck in context loops securely
- **Integration Visibility** — Enumerate secure connections to third-party apps like Slack, Gmail, and CRM systems to manage your AI's reach across your software stack
- **Workspace Management** — Navigate organizational boundaries and team structures to understand how Lindies are distributed across your company

### How it works

1. Subscribe to this server
2. Enter your Lindy API Token
3. Start managing your autonomous AI workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — automate repetitive workflows by triggering specialized Lindies and monitoring their execution history through natural conversation
- **Developers** — debug autonomous agent logic and inspect reasoning logs directly from your workspace without manual API testing
- **Founders & Leaders** — audit AI integrations and monitor the performance of your automated workforce across different team boundaries efficiently


## Available Tools (10)
- **cancel_run**: Cancel a running execution dispatching hard stops interrupting trapped context loops
- **get_run**: Get specific state for a Run blocking on Human input or External APIs
- **get_lindy**: Get configuration mappings including standard tools and prompts for a specific Lindy
- **list_integrations**: List bounded third-party app connections securely connected (e.g Slack, Gmail)
- **list_runs**: List recent runs validating the full execution graph isolating active Lindy instances
- **list_lindies**: List all custom autonomous AI Assistants (Lindies) built on the workspace
- **get_run_logs**: Dump literal LLM reasoning logs isolating a specific run loop
- **trigger_lindy**: Trigger a Lindy to start an asynchronous task run parsing a JSON payload
- **list_triggers**: List how autonomous AI agents are woken up (Cron, Webhook, API)
- **list_workspaces**: List all explicit organizational boundaries structuring isolated Teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lindy (Autonomous AI Employees)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Lindies in my workspace"

**🤖 AI Agent:**
> I've found 3 autonomous assistants: 'Sales-Research-Lindy' (ID: l-123), 'Customer-Support-Lindy' (ID: l-456), and 'Content-Writer-Lindy' (ID: l-789). Which one would you like to trigger or inspect?

---

**👤 You:**
> "Show me the reasoning logs for the last run of 'Sales-Research-Lindy'"

**🤖 AI Agent:**
> Retrieving logs for run ID 'run-98765'… I've extracted the reasoning steps. The Lindy searched for LinkedIn profiles, identified 5 targets, drafted personalized intro emails, and is now waiting for your approval to send them via Gmail. Would you like to see the draft email content?

---

**👤 You:**
> "What triggers are currently configured for our autonomous agents?"

**🤖 AI Agent:**
> I've identified 3 active triggers: 1) Webhook (ID: tr-123) for 'Support-Lindy', 2) Scheduled Cron (Daily at 9 AM) for 'Report-Lindy', and 3) Manual API trigger for all assistants. I can provide the specific webhook URLs if needed.


## ❓ FAQ

**Q: Can I see exactly how my Lindy made a specific decision?**
Yes. Use the `get_run_logs` tool with a specific Run ID. Your agent will retrieve the literal LLM reasoning loops and step-by-step validations, giving you full transparency into the autonomous agent's logic.

**Q: How do I trigger an autonomous task through a conversation?**
The `trigger_lindy` tool allows you to start an asynchronous task run. You just need to provide the Lindy ID and a JSON payload defining the inputs for the task. Your agent will fire the job and return a Run ID for status tracking.

**Q: Can my agent list which third-party apps my Lindies are connected to?**
Absolutely. Use the `list_integrations` tool to retrieve all active third-party app connections. Your agent will report which channels (like Slack, Gmail, or HubSpot) are securely connected to your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lindy-autonomous-ai-employees](https://vinkius.com/mcp/lindy-autonomous-ai-employees)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lindy (Autonomous AI Employees)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lindy-autonomous-ai-employees` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lindy (Autonomous AI Employees)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lindy-autonomous-ai-employees": {
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
