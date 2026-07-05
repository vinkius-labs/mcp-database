# Minimum Spanning Tree Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/minimum-spanning-tree-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate Minimum and Maximum Spanning Trees using Kruskal's and Prim's algorithms.

## Description
This MCP server provides algorithmic tools to find the Minimum Spanning Tree (MST) and Maximum Spanning Tree of a graph. Using `compute_kruskal_mst`, you can identify the lowest-weight edges that connect all nodes without cycles, which is ideal for network design. The `compute_prim_mst` tool allows you to grow a tree from a specific starting node by always selecting the cheapest available connection. For scenarios where you need to maximize connectivity weight, use `compute_max_spanning_tree`. All tools accept an edge list format and can identify if the resulting structure is a single tree or a spanning forest.


## Available Tools (3)
- **compute_kruskal_mst**: Calculates the Minimum Spanning Tree using Kruskal's algorithm
- **compute_max_spanning_tree**: Calculates the Maximum Spanning Tree
- **compute_prim_mst**: Calculintates the Minimum Spanning Tree using Prim's algorithm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Minimum Spanning Tree Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the MST for a graph with edges: [{'source': 'A', 'target': 'B', 'weight': 4}, {'source': 'B', 'target': 'C', 'weight': 1}, {'source': 'A', 'target': 'C', 'weight': 3}]"

**🤖 AI Agent:**
> The Minimum Spanning Tree edges are: [{'source': 'B', 'target': 'C', 'weight': 1}, {'source': 'A', 'target': 'C', 'weight': 3}]. Total weight is 4.

---

**👤 You:**
> "Calculate the Maximum Spanning Tree for edges: [{'source': 'Node1', 'target': 'Node2', 'weight': 10}, {'source': 'Node2', 'target': 'Node3', 'weight': 5}, {'source': 'Node1', 'target': 'Node3', 'weight': 2}]"

**🤖 AI Agent:**
> The Maximum Spanning Tree edges are: [{'source': 'Node1', 'target': 'Node2', 'weight': 10}, {'source': 'Node2', 'target': 'Node3', 'weight': 5}]. Total weight is 15.

---

**👤 You:**
> "Using Prim's algorithm, find the MST starting from node 'A' for edges: [{'source': 'A', 'target': 'B', 'weight': 2}, {'source': 'B', 'target': 'C', 'weight': 3}, {'source': 'A', 'target': 'C', 'weight': 5}]"

**🤖 AI Agent:**
> The Minimum Spanning Tree edges are: [{'source': 'A', 'target': 'B', 'weight': 2}, {'source': 'B', 'target': 'C', 'weight': 3}]. Total weight is 5.


## ❓ FAQ

**Q: What is the difference between Kruskal's and Prim's algorithms?**
Kruskal's algorithm sorts all edges by weight and adds them if they don't form a cycle, making it efficient for sparse graphs. Prim's algorithm starts from a specific node and expands the tree by picking the cheapest edge connected to the current tree.

**Q: How do I calculate a Maximum Spanning Tree?**
You can use the `compute_max_spanning_tree` tool. It internally negates the edge weights to apply MST logic, effectively finding the set of edges with the highest total weight.

**Q: What happens if my graph is disconnected?**
If the input graph has multiple components, the tools will return a spanning forest. The `isForest` property in the response will be set to true.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/minimum-spanning-tree-calculator](https://vinkius.com/mcp/minimum-spanning-tree-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Minimum Spanning Tree Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `minimum-spanning-tree-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Minimum Spanning Tree Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "minimum-spanning-tree-calculator": {
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
