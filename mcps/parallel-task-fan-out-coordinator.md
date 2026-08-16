# Parallel Task Fan-out Coordinator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/parallel-task-fan-out-coordinator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [orchestration](../categories/orchestration.md)

Synchronize parallel agentic workflows with deterministic barrier strategies.

## Description
This MCP server provides deterministic synchronization for parallel agentic workflows. It allows orchestrators to manage groups of concurrent tasks using specific coordination patterns. Use `register_task_batch` to initialize a group with a strategy like barrier, first_success, or quorum. You can track progress using `update_task_status` and check if the synchronization threshold is met via `get_batch_summary`. This is essential for managing complex fan-out/fan-in patterns in multi-agent systems.


## Available Tools (3)
- **get_batch_summary**: Retrieves the current orchestration state and results for a batch of tasks
- **register_task_batch**: Initializes a new group of tasks to be managed by the coordinator
- **update_task_status**: If status is COMPLETED, provide the result.

Reports the progress of an individual task to the coordinator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parallel Task Fan-out Coordinator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start a new batch of 3 tasks with a quorum requirement of 2."

**🤖 AI Agent:**
> Batch initialized with ID 'batch_123'. Total tasks: 3. Strategy: quorum. Quorum size: 2.

---

**👤 You:**
> "Update task 'task_A' to COMPLETED with the result 'success_data'."

**🤖 AI Agent:**
> Status updated. isThresholdMet: true. proceedReason: Quorum reached.

---

**👤 You:**
> "Get the summary for batch 'batch_123'."

**🤖 AI Agent:**
> Batch summary: shouldProceed: true, completedResults: { 'task_A': 'success_data' }, failedTaskIds: [].


## ❓ FAQ

**Q: What synchronization strategies are supported?**
The coordinator supports three strategies: barrier (waits for all tasks), first_success (proceeds after one success), and quorum (proceeds after a specific number of successes).

**Q: How do I check if my parallel tasks are finished?**
You can use `get_batch_summary` to retrieve the current state of the batch, including whether the synchronization threshold has been met and the results of completed tasks.

**Q: Can I set a timeout for a batch of tasks?**
Yes, when calling `register_task_batch`, you can provide a `maxWaitMs` parameter to enforce a deadline for the entire batch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/parallel-task-fan-out-coordinator](https://vinkius.com/ai-agent-connect/parallel-task-fan-out-coordinator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parallel Task Fan-out Coordinator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parallel-task-fan-out-coordinator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parallel Task Fan-out Coordinator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parallel-task-fan-out-coordinator": {
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
