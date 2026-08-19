# DAG Topological Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dag-topological-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Deterministic task scheduling and critical path analysis for multi-agent DAGs.

## Description
This MCP server provides a deterministic engine for multi-agent orchestration using Directed Acyclic Graphs (DAGs). It allows AI agents to calculate optimal task execution orders, identify the critical path, and manage parallel resource allocation. Using `analyze_dag_structure`, agents can validate graph integrity and detect cycles. The `calculate_slack_and_bottlenecks` tool identifies task flexibility and pinpoint bottlenecks, while `simulate_agent_schedule` calculates real-world makespan and parallelism efficiency for a given number of agents.


## Available Tools (3)
- **analyze_dag_structure**: Validates the integrity of the task graph and determines the core sequence and critical path
- **calculate_slack_and_bottlenecks**: Identifies task flexibility and pinpoints the most sensitive tasks in the workflow
- **simulate_agent_schedule**: Calculates the real-world execution timeline (makespan) and efficiency when limited agents are applied to the workload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DAG Topological Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this task list for cycles and the critical path: [{'id': 'A', 'durationMs': 100, 'dependencies': []}, {'id': 'B', 'durationMs': 200, 'dependencies': ['A']}, {'id': 'C', 'durationMs': 150, 'dependencies': ['A']}]"

**🤖 AI Agent:**
> The topological order is ['A', 'B', 'C'] or ['A', 'C', 'B']. The critical path is ['A', 'B'] with a duration of 300ms.

---

**👤 You:**
> "Simulate a schedule for these tasks with 2 agents: [{'id': 'T1', 'durationMs': 50, 'dependencies': []}, {'id': 'T2', 'durationMs': 50, 'dependencies': []}, {'id': 'T3', 'durationMs': 50, 'dependencies': ['T1', 'T2']}]"

**🤖 AI Agent:**
> With 2 agents, the makespan is 100ms. T1 and T2 start at 0ms, and T3 starts at 50ms.

---

**👤 You:**
> "Find the bottleneck tasks for this DAG: [{'id': '1', 'durationMs': 10, 'dependencies': []}, {'id': '2', 'durationMs': 20, 'dependencies': ['1']}, {'id': '3', 'durationMs': 5, 'dependencies': ['1']}]"

**🤖 AI Agent:**
> The bottleneck tasks are ['1', '2'] because they have zero slack time.


## ❓ FAQ

**Q: How does the scheduler handle parallel execution?**
The server uses list scheduling to assign ready tasks to available agents, prioritizing tasks on the critical path to minimize total makespan.

**Q: Can it detect errors in my task graph?**
Yes, by using `analyze_dag_structure`, the engine can detect if a graph contains cycles, which would make it an invalid DAG.

**Q: What is a bottleneck task?**
A bottleneck task is a task with zero slack time. Any delay in these tasks will directly delay the entire project completion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dag-topological-scheduler](https://vinkius.com/ai-agent-connect/dag-topological-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DAG Topological Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dag-topological-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DAG Topological Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dag-topological-scheduler": {
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
