# YepCode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yepcode)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Run serverless code snippets in the cloud with a platform that lets you build integrations and automations in any programming language.

## Description
Connect your **YepCode** account to any AI agent and simplify how you automate complex data integrations and serverless workflows through natural conversation.

### What you can do

- **Process Control** — List and trigger serverless processes with custom parameters directly from your agent.
- **Execution Monitoring** — Track the history and status of your workflow runs to ensure reliability.
- **Secret Management** — List and verify account secrets used in your automations without exposing values.
- **Team Coordination** — Query available teams and workspaces to understand your development environment.

### How it works

1. Subscribe to this server
2. Enter your YepCode API Key
3. Start running and monitoring your serverless automations from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly trigger maintenance workflows or data syncs via simple AI commands.
- **Data Analysts** — monitor the status of recurring ETL processes and verify secret availability.
- **Software Developers** — test and run serverless functions during the development cycle without leaving the IDE.


## Available Tools
- **get_process_details**: Get details for a specific process
- **list_executions**: List recent process executions
- **list_processes**: List YepCode processes
- **list_secrets**: List account secrets
- **list_teams**: List available teams
- **run_process**: Trigger a process execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YepCode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available processes in my YepCode account."

**🤖 AI Agent:**
> I've retrieved your processes. You have 5 serverless workflows configured, including 'Database Sync', 'PDF Generator', and 'Slack Notifier'. Which one would you like to run?

---

**👤 You:**
> "Run the 'Data Export' process with the parameter { "format": "csv" }."

**🤖 AI Agent:**
> Process triggered! The 'Data Export' execution has started with ID exe_12930. I'll let you know when the history shows it's complete.

---

**👤 You:**
> "Check the status of my recent process executions."

**🤖 AI Agent:**
> Inspecting recent executions... I found 3 entries: 'PDF Generator' (Success), 'Database Sync' (Success), and 'Web Scraper' (Error). Would you like the error logs for the Web Scraper?


## ❓ FAQ

**Q: Can I provide input parameters when running a process?**
Yes, the `run_process` tool accepts an optional JSON object for parameters, allowing you to pass dynamic data to your serverless functions.

**Q: How do I check if a process execution failed?**
Use the `list_executions` query. It will return a history of recent runs along with their final status (e.g., success, error, pending).

**Q: Is it possible to see the code of my processes via AI?**
Yes, you can use the `get_process_details` tool to retrieve the complete metadata and code configuration for any specific process ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yepcode](https://vinkius.com/mcp/yepcode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **YepCode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `yepcode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **YepCode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yepcode": {
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
