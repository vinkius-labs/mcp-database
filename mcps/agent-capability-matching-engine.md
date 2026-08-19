# Agent Capability Matching Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-capability-matching-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [routing](../categories/routing.md)

A deterministic routing engine that matches user intent to the optimal agent or sequence of agents.

## Description
This MCP server provides a decision-making layer to route tasks to the most suitable AI agents. It calculates optimal routing by analyzing capability intersection, performance metrics like success rate and latency, and real-time system load. Use `calculate_routing_scores` to find the best agent, `analyze_capability_gaps` to identify missing skills, `plan_multi_agent_composition` to chain multiple agents together, and `validate_routing_health` to ensure the routing plan is reliable.


## Available Tools (4)
- **analyze_capability_gaps**: Identifies what capabilities are missing from the agent pool to satisfy a specific intent
- **calculate_routing_scores**: Determines the optimal agent(s) for a specific user intent by calculating composite scores
- **plan_multi_agent_composition**: Determines the optimal sequence of agents required to fulfill an intent when no single agent is sufficient
- **validate_routing_health**: Checks if the current routing plan is risky due to low scores or high gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Capability Matching Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best agent for an intent requiring 'data_analysis' and 'sql_query' given a list of available agents."

**🤖 AI Agent:**
> The primary agent selected is agent_001 with a routing confidence of 0.85.

---

**👤 You:**
> "What capabilities are missing to fulfill the intent 'image_generation'?"

**🤖 AI Agent:**
> The missing capabilities are 'diffusion_model' and 'style_transfer'.

---

**👤 You:**
> "Plan a multi-agent sequence for a task requiring 'web_search' and 'file_writing'."

**🤖 AI Agent:**
> The optimal sequence is [search_agent_v2, file_manager_pro].


## ❓ FAQ

**Q: How does the engine select the best agent?**
The engine uses `calculate_routing_scores` to compute a composite score for each agent based on capability match, success rate, latency, and current system load.

**Q: What happens if no single agent has all the required capabilities?**
You can use `plan_multi_agent_composition` to identify the optimal sequence of multiple agents that, when combined, satisfy all requirements.

**Q: How can I check if a routing plan is reliable?**
Use the `validate_routing_health` tool to check if the routing plan is risky due to low scores or high capability gaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-capability-matching-engine](https://vinkius.com/ai-agent-connect/agent-capability-matching-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Capability Matching Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-capability-matching-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Capability Matching Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-capability-matching-engine": {
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
