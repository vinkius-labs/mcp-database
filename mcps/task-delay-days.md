# Task Delay Days MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/task-delay-days)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate project schedule variances and task delays.

## Description
This MCP server provides precision tools for measuring the temporal gap between planned and actual task completion. Use `get_task_delay` to find specific task variances, `get_batch_delay_summary` for high-level project health overviews, `check_schedule_compliance` to validate delays against tolerance thresholds, and `get_project_delay_trend` to analyze how delays accumulate monthly.


## Available Tools (4)
- **check_schedule_compliance**: Determines if a specific task or a set of tasks meets a predefined tolerance threshold for delays
- **get_batch_delay_summary**: Aggregates delay data across multiple tasks to provide a high-level overview of project health
- **get_project_delay_trend**: Analyzes how delays are accumulating over time by grouping task delays by their planned completion months
- **get_task_delay**: Calculates the specific number of days a single task is delayed or early


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Task Delay Days** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days was the task delayed if it was planned for 2024-05-01 and finished on 2024-05-05?"

**🤖 AI Agent:**
> The task was delayed by 4 days.

---

**👤 You:**
> "Is a task compliant if it was planned for 2024-06-10, finished on 2024-06-12, and my tolerance is 3 days?"

**🤖 AI Agent:**
> Yes, the task is compliant as the 2-day delay is within the 3-day tolerance.

---

**👤 You:**
> "What is the total delay for these tasks: [{ 'plannedDate': '2024-01-01', 'actualDate': '2024-01-05' }, { 'plannedDate': '2024-01-10', 'actualDate': '2024-01-08' }]?"

**🤖 AI Agent:**
> The total delay is 2 days.


## ❓ FAQ

**Q: How do I calculate the delay for a single task?**
You can use the `get_task_delay` tool by providing the planned completion date and the actual completion date in ISO 8601 format.

**Q: Can I check if my project is within its allowed delay threshold?**
Yes, the `check_schedule_compliance` tool allows you to define a tolerance in days to see if a task is compliant or exceeds the limit.

**Q: How can I see the trend of delays over several months?**
The `get_project_delay_trend` tool aggregates task delays and groups them by the month of their planned completion date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/task-delay-days](https://vinkius.com/en/ai-agent-connect/task-delay-days)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Task Delay Days** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `task-delay-days` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Task Delay Days** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-delay-days": {
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
