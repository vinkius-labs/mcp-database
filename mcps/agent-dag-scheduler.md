# Agent DAG Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-dag-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A deterministic engine for calculating execution order and scheduling metrics for multi-agent workflows.

## Description
This MCP server provides a deterministic execution engine for multi-agent workflows based on Directed Acyclic Graphs (DAGs). It allows AI agents to calculate the exact execution order using topological sort, determine the critical path duration, and simulate wall-clock time based on available parallel slots. Use `analyze_workflow_structure` to validate graph integrity and detect cycles, `simulate_execution_schedule` to model resource utilization and efficiency, or `get_task_timing_details` to inspect specific temporal constraints like slack time.


## Available Tools (3)
- **analyze_workflow_structure**: Validates the integrity of the provided task graph and determines the fundamental execution sequence
- **get_task_timing_details**: Provides a deep dive into the temporal constraints of a specific task within a specific schedule
- **simulate_execution_schedule**: Calculates the actual timing and resource utilization of the workflow given a limited number of execution slots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent DAG Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this set of tasks is a valid DAG: [{'id': 'A', 'duration': 10, 'deps': []}, {'id': 'B', 'duration': 5, 'deps': ['A']}, {'id': 'A', 'duration': 10, 'deps': ['B']}]"

**🤖 AI Agent:**
> {"is_dag": false, "cycle_path": ["A", "B", "A"]}

---

**👤 You:**
> "Simulate a schedule for these tasks with 2 parallel slots: [{'id': 'T1', 'duration': 10, 'deps': []}, {'id': 'T2', 'duration': 10, 'deps': []}, {'id': 'T3', 'duration': 10, 'deps': ['T1', 'T2']}]"

**🤖 AI Agent:**
> {"wall_clock_time": 20, "efficiency": 0.5}

---

**👤 You:**
> "What is the slack time for task T2 in this schedule?"

**🤖 AI Agent:**
> {"task_id": "T2", "duration": 10, "earliest_start": 0, "latest_start": 0, "slack_time": 0}


## ❓ FAQ

**Q: How does the scheduler handle parallel execution?**
The `simulate_execution_schedule` tool calculates how tasks are distributed across a specified number of parallel slots, accounting for both dependency constraints and resource availability.

**Q: Can this tool detect errors in my workflow structure?**
Yes, by using `analyze_workflow_structure`, the engine validates if the task graph is a valid DAG and will return the specific cycle path if a loop is detected.

**Q: What is the difference between critical path and wall-clock time?**
The critical path is the longest sequence of dependent tasks, representing the absolute minimum time needed. Wall-clock time is the actual elapsed time when limited parallel slots are applied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-dag-scheduler](https://vinkius.com/ai-agent-connect/agent-dag-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent DAG Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-dag-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent DAG Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-dag-scheduler": {
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
