# Classroom Project Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/classroom-project-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize classroom group projects by managing tasks, student workloads, and milestones.

## Description
Classroom Project Planner helps educators manage complex group assignments. Use `get_project_overview` to see the big picture, `list_task_dependencies` to identify blockers, `get_student_workload` to prevent student burnout, and `check_milestone_readiness` to track progress toward key project goals.


## Available Tools (4)
- **check_milestone_readiness**: Determines if all requirements for a specific milestone have been met
- **get_project_overview**: Provides a high-level summary of the entire project status
- **get_student_workload**: Checks how much work is assigned to a specific student to prevent burnout
- **list_task_dependencies**: Answers which tasks are blocking others to identify the critical path


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Classroom Project Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me an overview of project PROJ-123."

**🤖 AI Agent:**
> Project 'Science Fair' has 10 total tasks, 4 completed, and a total effort of 25 units. Scheduled milestones include 'Research Phase' on Oct 12th.

---

**👤 You:**
> "Is student STU-456 overloaded in project PROJ-123?"

**🤖 AI Agent:**
> Student Alex has 12 units of effort assigned across 3 tasks.

---

**👤 You:**
> "Is the 'Final Presentation' milestone ready in project PROJ-123?"

**🤖 AI Agent:**
> No, the milestone is not reached yet. There are 2 remaining tasks and 1 overdue task.


## ❓ FAQ

**Q: How can I see if a student has too much work?**
You can use the `get_student_workload` tool to check the total effort and task count assigned to a specific student.

**Q: How do I know if a project milestone is complete?**
Use `check_milestone_readiness` to determine if all tasks for a milestone are finished.

**Q: Can I see which tasks are blocking my project progress?**
Yes, the `list_task_dependencies` tool identifies which tasks are currently blocking others.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/classroom-project-planner](https://vinkius.com/en/ai-agent-connect/classroom-project-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Classroom Project Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `classroom-project-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Classroom Project Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "classroom-project-planner": {
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
