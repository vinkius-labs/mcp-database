# CrewAI Task Dependency Graph Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crewai-task-dependency-graph-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [graph-theory](../categories/graph-theory.md)

Ensures multi-agent task sequences are free of circular logic and properly ordered.

## Description
The CrewAI Task Dependency Graph Validator is a specialized engine designed to ensure that complex, multi-agent workflows in CrewAI are executed in the correct order. By modeling tasks as nodes in a Directed Acyclic Graph (DAG), it uses Kahn's algorithm to detect circular dependencies and determine the optimal execution sequence. Use `validate_task_graph` to check for loops, `audit_context_integrity` to find broken task links, and `calculate_task_complexity` to measure the downstream impact of specific tasks.


## Available Tools (3)
- **audit_context_integrity**: Audits the integrity of task context references
- **calculate_task_complexity**: Calculates the complexity of a task within a graph
- **validate_task_graph**: Validates a task graph for circular dependencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrewAI Task Dependency Graph Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this task list has any circular dependencies: [{'id': 'task1', 'dependencies': ['task2']}, {'id': 'task2', 'dependencies': ['task1']}]"

**🤖 AI Agent:**
> The task graph is invalid. The following cyclic dependencies were detected: ['task1', 'task2'].

---

**👤 You:**
> "What is the impact of failing 'research_task' in my workflow?"

**🤖 AI Agent:**
> Failing 'research_task' will have a downstream impact count of 3, affecting all tasks that depend on its output.

---

**👤 You:**
> "Verify if all context references in my task list are correct."

**🤖 AI Agent:**
> The integrity check passed. All tasks listed in `contextFrom` fields exist within the provided registry.


## ❓ FAQ

**Q: What is the purpose of this MCP server?**
It validates that your CrewAI task sequences do not contain circular dependencies and are properly ordered for execution.

**Q: How can I detect if a task is causing a loop?**
You can use the `validate_task_graph` tool. If it returns a non-empty `cyclicDependencies` list, those tasks are part of a loop.

**Q: Can I check if all my task references are valid?**
Yes, the `audit_context_integrity` tool will identify any tasks that attempt to pull context from non-existent tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crewai-task-dependency-graph-validator](https://vinkius.com/ai-agent-connect/crewai-task-dependency-graph-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrewAI Task Dependency Graph Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crewai-task-dependency-graph-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrewAI Task Dependency Graph Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crewai-task-dependency-graph-validator": {
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
