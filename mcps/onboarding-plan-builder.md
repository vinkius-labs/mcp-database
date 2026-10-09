# Onboarding Plan Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/onboarding-plan-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured, actionable first-month onboarding schedules.

## Description
This MCP server provides tools to manage the entire first-month onboarding lifecycle. It allows AI agents to use `get_onboarding_plan` to retrieve schedules, `add_onboarding_task` to append new requirements across training, meetings, documents, and access pillars, `update_task_status` to track progress, and `validate_plan_readiness` to ensure all necessary tasks are completed before a new hire begins.


## Available Tools (4)
- **get_onboarding_plan**: Retrieves a complete, structured onboarding plan for a specific employee
- **add_onboarding_task**: Appends a new requirement to an existing onboarding plan
- **update_task_status**: Marks a specific task as finished or in progress
- **validate_plan_readiness**: Checks if an onboarding plan is complete and ready for the employee to begin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Onboarding Plan Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the onboarding plan for employee ID 12345."

**🤖 AI Agent:**
> The onboarding plan for employee 12345 includes 5 tasks: 1 Training, 1 Meeting, 2 Documents, and 1 Access task.

---

**👤 You:**
> "Add a meeting task for employee 12345 with owner 'HR Team' due on 2025-02-15."

**🤖 AI Agent:**
> The meeting task has been successfully added to the plan for employee 12345.

---

**👤 You:**
> "Is the onboarding plan for employee 12345 ready?"

**🤖 AI Agent:**
> The plan is ready. All required task types are present and no tasks are overdue.


## ❓ FAQ

**Q: How can I see the current onboarding progress?**
You can use the `get_onboarding_plan` tool to retrieve the full structured plan, including the status of every task.

**Q: Can I add new tasks to an existing plan?**
Yes, use the `add_onboarding_task` tool to add new training, meeting, document, or access requirements.

**Q: How do I know if a new hire is ready to start?**
Use the `validate_plan_readiness` tool. It checks if all required task types are present and if any tasks are overdue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/onboarding-plan-builder](https://vinkius.com/en/ai-agent-connect/onboarding-plan-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Onboarding Plan Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onboarding-plan-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Onboarding Plan Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onboarding-plan-builder": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
