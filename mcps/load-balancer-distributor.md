# Load Balancer Distributor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/load-balancer-distributor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic simulation engine for evaluating load balancing algorithms.

## Description
This MCP server provides a deterministic simulation engine to evaluate how various load-balancing algorithms distribute weighted tasks across a pool of agents. Use `simulate_distribution` to calculate exact task-to-agent assignments and performance metrics like load variance and saturation. You can also use `get_agent_status` to inspect agent utilization or `validate_system_constraints` to verify if a distribution plan is feasible without exceeding agent capacities.


## Available Tools (3)
- **simulate_distribution**: Calculates the exact assignment of tasks to agents using a specific algorithm and returns performance metrics
- **validate_system_constraints**: Checks if a proposed set of tasks can be distributed without any agent exceeding its absolute capacity
- **get_agent_status**: Provides a snapshot of the current state of all agents to prepare for a simulation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Load Balancer Distributor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate a distribution using round_robin for these agents: [{'id': 'a1', 'capacity': 100, 'currentLoad': 10, 'latencyMs': 5}] and these tasks: [{'id': 't1', 'weight': 20, 'affinityKey': 'k1'}]"

**🤖 AI Agent:**
> { "assignments": [ { "taskId": "t1", "agentId": "a1" } ], "loadVariance": 0, "maxLoadRatio": 0.3, "affinityPreservation": 100, "isSaturated": false }

---

**👤 You:**
> "Check the status of agent 'a1'."

**🤖 AI Agent:**
> { "agentId": "a1", "utilization": 0.1, "totalLoad": 10 }

---

**👤 You:**
> "Is it feasible to assign a task with weight 95 to an agent with capacity 100 and current load 10 using least_connections?"

**🤖 AI Agent:**
> { "isFeasible": false, "bottleneckAgentId": "a1" }


## ❓ FAQ

**Q: What algorithms are supported?**
The engine supports round_robin, weighted_round_robin, least_connections, consistent_hash, and power_of_two_choices.

**Q: How is saturation determined?**
A saturation flag is triggered if any agent's total load (existing load plus new task weights) exceeds 90% of its maximum capacity.

**Q: Can I check if a distribution is feasible?**
Yes, use the `validate_system_constraints` tool to check if a proposed set of tasks can be distributed without exceeding any agent's absolute capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/load-balancer-distributor](https://vinkius.com/ai-agent-connect/load-balancer-distributor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Load Balancer Distributor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `load-balancer-distributor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Load Balancer Distributor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "load-balancer-distributor": {
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
