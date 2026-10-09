# side-project-launch-plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/side-project-launch-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A scheduling engine that transforms task lists and effort estimates into realistic project timelines.

## Description
This MCP server provides a powerful scheduling engine for managing side projects. It calculates critical paths, identifies workload bottlenecks, and generates realistic timelines based on your weekly availability. Use `get_task_list` to view your project inventory, `calculate_schedule` to determine your completion date, and `analyze_workload_bottlenecks` to find weeks where your workload exceeds your capacity. It is designed to help you manage effort vs. duration and ensure your target launch date is achievable.


## Available Tools (4)
- **calculate_schedule**: Generates a timeline of tasks based on work capacity and dependencies
- **get_project_summary**: Provides a high-level overview of project health and progress
- **get_task_list**: You can filter by category.

Retrieves the current inventory of tasks and their properties
- **analyze_workload_bottlenecks**: Identifies specific weeks where the required effort exceeds the user's weekly capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **side-project-launch-plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the tasks I have planned for this project."

**🤖 AI Agent:**
> Here is your current task list: 1. Engine implementation (10h), 2. Database schema (5h), 3. Unit testing (8h).

---

**👤 You:**
> "What is my project timeline if I can work 10 hours per week?"

**🤖 AI Agent:**
> Based on 10 hours per week, your project is estimated to complete on 2024-12-15. The project is feasible for your target date.

---

**👤 You:**
> "Give me a summary of the project status."

**🤖 AI Agent:**
> Project Summary: Total effort is 45 hours, total duration is 14 days, and there are 12 tasks in total.


## ❓ FAQ

**Q: How does the engine calculate the project completion date?**
The engine uses `calculate_schedule` to process your task list, dependencies, and weekly hours to determine the earliest possible completion date based on the critical path.

**Q: Can I see which tasks are on the critical path?**
Yes, when you run `calculate_schedule`, the returned timeline includes an `isCritical` flag for each task to identify the critical path.

**Q: How do I identify if I am overworking in a specific week?**
You can use the `analyze_workload_bottlenecks` tool to identify specific weeks where the required effort exceeds your defined weekly capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/side-project-launch-plan](https://vinkius.com/en/ai-agent-connect/side-project-launch-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **side-project-launch-plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `side-project-launch-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **side-project-launch-plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "side-project-launch-plan": {
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
