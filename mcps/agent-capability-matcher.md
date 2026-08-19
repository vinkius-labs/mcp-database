# Agent Capability Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-capability-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-agents](../categories/ai-agents.md)

Optimizes task assignment to agents using capability matching and load balancing.

## Description
This MCP server provides deterministic bipartite matching to connect tasks with the most suitable agents. It uses strategies like greedy, hungarian, and priority-weighted to ensure tasks are assigned to agents possessing all required capabilities while maintaining optimal workload distribution. Use `match_tasks` to perform assignments, `validate_system_health` to monitor unassigned ratios and agent loads, and `get_capability_stats` to analyze skill coverage across your agent pool.


## Available Tools (3)
- **get_capability_stats**: Provides a summary of capability coverage across the entire agent pool
- **match_tasks**: Executes the core matching logic to pair tasks with agents based on a specific strategy
- **validate_system_health**: Evaluates the quality of the matching result by checking against predefined operational thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Capability Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Match these tasks to the available agents using the greedy strategy."

**🤖 AI Agent:**
> Task 'Data Analysis' has been assigned to Agent 'Alpha' with a match score of 0.85.

---

**👤 You:**
> "Check the current health of the matching system."

**🤖 AI Agent:**
> The system is healthy. Unassigned task ratio is 5% and all agent loads are below 95%.

---

**👤 You:**
> "Show me the capability distribution for all agents."

**🤖 AI Agent:**
> There are 12 unique capabilities. 'Python' is possessed by 8 agents, and 'Data Science' is possessed by 5 agents.


## ❓ FAQ

**Q: How does the matching logic work?**
The system uses the `match_tasks` tool to pair tasks with agents. An agent is only eligible if they possess every capability required by the task. The match score is then calculated based on capability alignment and current agent load.

**Q: How can I check if my agent pool is overloaded?**
You can use the `validate_system_health` tool. It flags the system as unhealthy if more than 20% of tasks are unassigned or if any agent's load exceeds 95%.

**Q: What are the available matching strategies?**
The server supports three strategies: GREEDY for fast local optimization, HUNGARIAN for global optimal matching, and PRIORITY_WEIGHTED to respect task importance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-capability-matcher](https://vinkius.com/ai-agent-connect/agent-capability-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Capability Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-capability-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Capability Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-capability-matcher": {
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
