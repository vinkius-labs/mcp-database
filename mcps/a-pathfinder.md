# A* Pathfinder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/a-pathfinder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [algorithms](../categories/algorithms.md)

Deterministic A* pathfinding for grid-based navigation.

## Description
This MCP server provides deterministic A* pathfinding capabilities for agents navigating 2D grid environments. It allows for precise movement planning using 4-directional or 8-directional movement types and various heuristics like Manhattan, Euclidean, or Chebyshev. Use `find_shortest_path` to calculate the most efficient route, `find_k_shortest_paths` to discover alternative routes, or `analyze_grid_feasibility` to validate if a path is possible before starting complex computations.


## Available Tools (3)
- **analyze_grid_feasibility**: 
- **find_k_shortest_paths**: 
- **find_shortest_path**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **A* Pathfinder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the shortest path in this 3x3 grid: [[0,0,0],[1,1,0],[0,0,0]] from [0,0] to [2,2] using 4-directional movement and manhattan heuristic."

**🤖 AI Agent:**
> [ [0,0], [0,1], [0,2], [1,2], [2,2] ]

---

**👤 You:**
> "Is it possible to move from [0,0] to [2,2] in a grid where [1,1] is an obstacle?"

**🤖 AI Agent:**
> Yes, a path is possible by navigating around the obstacle at [1,1].

---

**👤 You:**
> "Give me 2 alternative paths for a 5x5 grid from [0,0] to [4,4] using 8-directional movement."

**🤖 AI Agent:**
> Path 1: [[0,0], [1,1], [2,2], [3,3], [4,4]]. Path 2: [[0,0], [0,1], [1,2], [2,3], [3,4], [4,4]].


## ❓ FAQ

**Q: What movement types are supported?**
The server supports both 4-directional (cardinal) and 8-directional (cardinal and diagonal) movement.

**Q: How can I check if a path is possible without calculating it?**
You can use the `analyze_grid_feasibility` tool to quickly validate if a start and goal are reachable within the grid.

**Q: Is the pathfinding guaranteed to be optimal?**
Yes, when using an admissible heuristic like Manhattan or Euclidean distance, the `find_shortest_path` tool is guaranteed to find the optimal path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/a-pathfinder](https://vinkius.com/ai-agent-connect/a-pathfinder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **A* Pathfinder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `a-pathfinder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **A* Pathfinder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "a-pathfinder": {
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
