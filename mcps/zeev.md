# Zeev MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zeev)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Digitize business processes with BPMN workflows, electronic forms, and approval chains that replace paper and email chaos.

## Description
### What you can do
- List and manage your pending tasks in real-time.
- Start new process requests with custom form data.
- Complete tasks and make decisions directly from your AI agent.
- Delegate tasks to other team members and track process history.

### How it works
1. Get your Zeev domain and API Key from your profile settings.
2. Enter your credentials in Vinkius platform.
3. Start chatting with your Zeev agent to manage your workflows.

### Who is it for?
- Process managers looking for automated workflow control.
- Operations teams needing quick task execution.
- Developers integrating BPM into their AI-driven applications.


## Available Tools (11)
- **cancel_request**: Cancel an active process request
- **create_request**: Start a new process request in Zeev
- **delegate_task**: Delegate a task to another user
- **finish_task**: Finish/Complete a Zeev task
- **get_me**: Get current user information
- **get_process**: Get details of a process definition
- **get_request**: Get details of a specific process request
- **get_task**: Get details of a specific Zeev task
- **list_processes**: List available process definitions
- **list_requests**: List process requests (instances) in Zeev
- **list_tasks**: List pending tasks in Zeev


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zeev** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my pending tasks in Zeev."

**🤖 AI Agent:**
> I've found 3 pending tasks: 1. Approve Expense (ID: 123), 2. Review Contract (ID: 124), 3. Weekly Report (ID: 125).

---

**👤 You:**
> "Finish task 123 with decision 'Approved'."

**🤖 AI Agent:**
> Task 123 has been successfully completed with the decision 'Approved'.

---

**👤 You:**
> "Start a new 'Expense Report' process."

**🤖 AI Agent:**
> I've started a new 'Expense Report' request with ID 456.


## ❓ FAQ

**Q: Can I start any process using the AI agent?**
Yes, as long as you have the process ID and the required initial form data.

**Q: Is it possible to delegate tasks to specific users?**
Yes, you can use the delegate_task tool by providing the Task ID and the target User ID.

**Q: Can I see the history of a request?**
Yes, the get_request tool provides details including the current status and history of the instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeev](https://vinkius.com/mcp/zeev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zeev** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zeev` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zeev** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zeev": {
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
