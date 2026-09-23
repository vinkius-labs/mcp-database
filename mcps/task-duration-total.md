# task-duration-total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/task-duration-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregates and analyzes task durations for workload insights.

## Description
This MCP server provides a specialized calculation engine for aggregating and analyzing time durations assigned to various tasks. It allows AI agents to calculate total time spent on specific task sets using `get_total_duration`, sum durations by category via `get_category_duration`, and retrieve detailed statistical insights like average and extreme durations through `get_task_density_metrics`. For a high-level overview of the entire system, use `get_workload_summary` to see total workload and task counts.


## Available Tools (4)
- **get_category_duration**: Sums the durations of all tasks belonging to a specific category
- **get_task_density_metrics**: Provides analytical insights into how time is distributed across tasks
- **get_total_duration**: Calculates the sum of durations for a specific subset of tasks
- **get_workload_summary**: Returns a high-level overview of total time spent across all registered tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **task-duration-total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total time spent on tasks T1, T2, and T3?"

**🤖 AI Agent:**
> The total duration for tasks T1, T2, and T3 is 3600 seconds.

---

**👤 You:**
> "How much time has been spent on the 'development' category?"

**🤖 AI Agent:**
> The total time spent in the development category is 15400 seconds.

---

**👤 You:**
> "Give me a summary of the total workload in the system."

**🤖 AI Agent:**
> The system currently has a total workload of 85000 seconds across 42 registered tasks.


## ❓ FAQ

**Q: How can I find the total time spent on a specific group of tasks?**
You can use the `get_total_duration` tool by providing the list of task IDs you wish to sum.

**Q: Can I see how much time is spent in a specific category?**
Yes, the `get_category_duration` tool allows you to aggregate all durations for any valid category name.

**Q: What kind of statistical data can I get for my tasks?**
The `get_task_density_metrics` tool provides the average, maximum, and minimum durations, as well as the total duration for a set of tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/task-duration-total](https://vinkius.com/en/ai-agent-connect/task-duration-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **task-duration-total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `task-duration-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **task-duration-total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-duration-total": {
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
