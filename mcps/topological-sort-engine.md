# Topological Sort Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/topological-sort-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [algorithms](../categories/algorithms.md)

Perform topological sorting on DAGs using Kahn's and DFS algorithms to resolve dependencies and detect cycles.

## Description
The Topological Sort Engine provides specialized tools for managing directed acyclic graphs (DAGs). By utilizing `calculate_kahn_sort`, you can generate a linear execution order based on in-degree reduction. For alternative traversal methods, `calculate_dfs_sort` uses depth-first search to reconstruct task sequences. If your graph contains circular dependencies that prevent sorting, use `identify_cycles` to pinpoint the exact nodes involved in the loops. This engine is ideal for task scheduling, build system orchestration, and resolving complex prerequisite chains.


## Available Tools (3)
- **calculate_dfs_sort**: Generate a valid execution order using DFS-based approach
- **identify_cycles**: Isolate and list all nodes that are part of circular dependencies
- **calculate_kahn_sort**: Generate a valid linear execution order using Kahn's Algorithm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Topological Sort Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Using `calculate_kahn_sort`, what is the execution order for nodes ['A', 'B', 'C'] with edges [['A', 'B'], ['B', 'C']]?"

**🤖 AI Agent:**
> The valid execution order is: A, B, C.

---

**👤 You:**
> "I have a dependency loop between Task 1 and Task 2. Which tool should I use to find the nodes?"

**🤖 AI Agent:**
> You should use the `identify_cycles` tool to list all nodes involved in the circular dependency.

---

**👤 You:**
> "Check if this dependency chain is valid: nodes ['Task1', 'Task2'], edges [['Task1', 'Task2'], ['Task2', 'Task1']]"

**🤖 AI Agent:**
> The graph contains a cycle involving Task1 and Task2, so a topological sort is not possible.


## ❓ FAQ

**Q: What is the difference between Kahn's algorithm and DFS-based sorting?**
Kahn's algorithm uses an in-degree reduction approach (BFS), while the DFS-based method explores paths deeply before backtracking to reconstruct the sequence.

**Q: How can I find nodes that are causing a circular dependency?**
You can use the `identify_cycles` tool, which specifically traverses the graph to isolate and return only the nodes involved in loops.

**Q: What happens if my input graph is not a DAG?**
If a cycle is detected, the sorting tools will return a failure state with an error message describing the nature of the loop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/topological-sort-engine](https://vinkius.com/mcp/topological-sort-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Topological Sort Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `topological-sort-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Topological Sort Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "topological-sort-engine": {
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
