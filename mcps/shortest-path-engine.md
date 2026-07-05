# Shortest Path Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shortest-path-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [algorithms](../categories/algorithms.md)

Find optimal paths in weighted graphs using Dijkstra, A*, and Bellman-Ford algorithms.

## Description
The Shortest Path Engine provides specialized computational tools for navigating complex networks. Use `dijkstra` to find the most efficient route in graphs with non-negative weights. For optimized searches using spatial heuristics like Euclidean or Manhattan distances, use `astar`. If your graph contains negative edge weights or you need to detect infinite cost-reduction loops (negative cycles), use `bellman_ford`. This engine calculates precise paths, total distances, and reachability maps for any weighted directed or undirected graph.


## Available Tools (3)
- **astar**: Do NOT use for simple unweighted graphs.

Find the shortest path using A* search
- **bellman_ford**: Scan graph using Bellman-Ford algorithm
- **dijkstra**: Do NOT use for negative weights.

Find the shortest path using Dijkstra algorithm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shortest Path Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the shortest path from node 'A' to node 'C' using Dijkstra with these edges: [{'startNode': 'A', 'endNode': 'B', 'weight': 5}, {'startNode': 'B', 'endNode': 'C', 'weight': 3}, {'startNode': 'A', 'endNode': 'C', 'weight': 10}]"

**🤖 AI Agent:**
> The shortest path from A to C is [A, B, C] with a total distance of 8.

---

**👤 You:**
> "Using A* search with Manhattan heuristic, what is the path from 'Start' to 'End' in this graph: nodes=['Start', 'Mid', 'End'], edges=[{'startNode': 'Start', 'endNode': 'Mid', 'weight': 2}, {'startNode': 'Mid', 'endNode': 'End', 'weight': 2}]"

**🤖 AI Agent:**
> The optimal path from Start to End is [Start, Mid, End] with a total distance of 4.

---

**👤 You:**
> "Check for negative cycles in a graph starting from node 'S' with edges: [{'startNode': 'S', 'endNode': 'A', 'weight': 1}, {'startNode': 'A', 'endNode': 'B', 'weight': -2}, {'startNode': 'B', 'endNode': 'S', 'weight': 1}]"

**🤖 AI Agent:**
> A negative cycle was detected in the graph (S -> A -> B -> S has a total weight of 0, but if weights were lower, it would trigger). In this specific case, no infinite loop was found as the sum is exactly 0.


## ❓ FAQ

**Q: When should I use the Dijkstra tool?**
Use `dijkstra` when you are certain that all edge weights in your graph are zero or positive. It is highly efficient for standard shortest-path queries.

**Q: Can I use A* search without a heuristic?**
The `astar` tool requires a valid `heuristicType` (either `EUCLIDEAN` or `MANSDT`) to guide its search. Without a spatial estimate, the algorithm cannot function as intended.

**Q: How does the engine handle negative edge weights?**
For graphs with negative weights, you must use `bellman_ford`. This tool is specifically designed to process negative edges and identify if a negative cycle exists in your graph.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shortest-path-engine](https://vinkius.com/mcp/shortest-path-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shortest Path Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shortest-path-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shortest Path Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shortest-path-engine": {
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
