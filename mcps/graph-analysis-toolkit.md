# Graph Analysis Toolkit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/graph-analysis-toolkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Deep structural analysis of directed and undirected graphs, providing metrics on connectivity, topology, and node importance.

## Description
The Graph Analysis Toolkit is a specialized engine for deep structural analysis of directed and undirected graphs. It provides essential metrics including degree (in-degree and out-degree), density, connected components, and strongly connected components using Tarjan's algorithm. You can also identify structural vulnerabilities like articulation points and bridges, calculate centrality measures such as degree and betweenness centrality approximation, and perform isomorphism checks for small graphs. Use `get_node_degrees` to find connection counts, `analyze_graph_connectivity` for connectivity metrics, `detect_structural_vulnerabilities` for critical nodes/edges, `calculate_centrality_metrics` for node importance, and `check_graph_isomorphism` to compare graph structures.


## Available Tools (5)
- **analyze_graph_connectivity**: Assess graph interconnectedness and identify isolated groups
- **calculate_centrality_metrics**: Rank nodes based on influence and position
- **check_graph_isomorphism**: Determine if two graphs are structurally identical
- **detect_structural_vulnerabilities**: Identify critical nodes and edges that break connectivity
- **get_node_degrees**: Determine incoming and outgoing connections for nodes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Graph Analysis Toolkit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the degree of node 'A' in this graph: {"nodes":["A","B"],"edges":[["A","B"]],"type":"undirected"}?"

**🤖 AI Agent:**
> Node 'A' has an in-degree of 1 and an out-degree of 1.

---

**👤 You:**
> "Check if these two graphs are structurally identical: Graph 1: {"nodes":["1","2"],"edges":[["1","2"]],"type":"undirected"} and Graph 2: {"nodes":["A","B"],"edges":[["A","B"]],"type":"undirected"}"

**🤖 AI Agent:**
> Yes, the two graphs are isomorphic.

---

**👤 You:**
> "Find the most influential nodes in this graph: {"nodes":["A","B","C"],"edges":[["A","B"],["B","C"]],"type":"directed"}"

**🤖 AI Agent:**
> Node 'B' has the highest centrality as it acts as a bridge between 'A' and 'C'.


## ❓ FAQ

**Q: How do I find the number of connections for a specific node?**
Use the `get_node_degrees` tool and provide the JSON string of your graph along with an array of the node IDs you want to check.

**Q: Can I identify critical points that might break my network?**
Yes, the `detect_structural_vulnerabilities` tool identifies articulation points and bridges that would disconnect parts of your graph if removed.

**Q: Is there a limit to the size of graphs I can compare for isomorphism?**
The `check_graph_isomorphism` tool is designed for small graphs. Comparing very large graphs may result in a complexity error due to performance constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/graph-analysis-toolkit](https://vinkius.com/mcp/graph-analysis-toolkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Graph Analysis Toolkit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graph-analysis-toolkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Graph Analysis Toolkit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graph-analysis-toolkit": {
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
