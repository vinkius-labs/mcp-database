# Task DAG Dependency Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/task-dag-dependency-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Resolves task execution order and parallel groups from DAG dependencies.

## Description
This MCP server provides advanced graph mathematics for agentic orchestration. It uses Kahn's algorithm to calculate valid execution sequences and identify tasks that can run in parallel. Use `resolve_execution_order` to get a full execution plan, `detect_cycles` to find deadlocks in your pipeline, or `find_isolated_tasks` to identify disconnected nodes. It is designed for managing complex task dependencies in frameworks like CrewAI or LangGraph.


## Available Tools (3)
- **find_isolated_tasks**: Identifies tasks that are completely disconnected from the rest of the execution graph
- **resolve_execution_order**: Calculates the valid execution sequence and parallel execution groups for a set of tasks
- **detect_cycles**: Specifically focuses on finding and describing the exact loop causing a deadlock in the pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Task DAG Dependency Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the execution order for these tasks: TaskA depends on TaskB, TaskB depends on TaskC."

**🤖 AI Agent:**
> The valid execution order is TaskC, then TaskB, then TaskA.

---

**👤 You:**
> "Check if there is a cycle in this task list: A depends on B, B depends on A."

**🤖 AI Agent:**
> Yes, a circular dependency was detected: ["A", "B", "A"].

---

**👤 You:**
> "Find all isolated tasks in a graph where TaskA and TaskB are connected, but TaskC has no dependencies."

**🤖 AI Agent:**
> The isolated task is TaskC.


## ❓ FAQ

**Q: How do I find tasks that can run at the same time?**
You can use the `resolve_execution_order` tool, which returns `parallelGroups` containing sets of task IDs that share the same depth level in the dependency graph.

**Q: What happens if my task list has a circular dependency?**
If a cycle is detected, you can use `detect_cycles` to retrieve the exact `cyclePath` that forms the loop, allowing you to fix the deadlock.

**Q: Can I use this for LangGraph or CrewAI workflows?**
Yes, this server is specifically built to resolve execution orders for agentic pipelines like those used in LangGraph and CrewAI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/task-dag-dependency-resolver](https://vinkius.com/ai-agent-connect/task-dag-dependency-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Task DAG Dependency Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `task-dag-dependency-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Task DAG Dependency Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-dag-dependency-resolver": {
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
