# Zeev MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zeev)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zeev-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zeev-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Zeev** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zeev](https://vinkius.com/mcp/zeev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
