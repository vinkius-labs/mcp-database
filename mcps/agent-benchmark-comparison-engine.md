# Agent Benchmark Comparison Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-benchmark-comparison-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

A deterministic engine for ranking and comparing LLM agents based on performance metrics.

## Description
The Agent Benchmark Comparison Engine provides a mathematical framework to evaluate LLM agents. By normalizing metrics like accuracy, latency, cost, and hallucination rates, it calculates a precise composite score for each agent. Use `calculate_agent_rankings` to generate ranked lists based on custom weights, `get_agent_performance_summary` to identify leaders in specific categories, or `validate_benchmark_config` to ensure your evaluation parameters are mathematically sound.


## Available Tools (3)
- **calculate_agent_rankings**: Performs the complete mathematical comparison and ranking of a set of agents based on provided weights
- **get_agent_performance_summary**: Retrieves a high-level overview of the best-performing agents for specific use cases
- **validate_benchmark_config**: 0 and metrics are within logical bounds.

Ensures that a proposed set of weights and agent metrics are mathematically valid before running heavy calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Benchmark Comparison Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these agents: AgentA (accuracy: 90, latency: 200, cost: 0.5, hallucination: 0.02), AgentB (accuracy: 85, latency: 150, cost: 0.3, hallucination: 0.05) with weights accuracy: 0.4, latency: 0.3, cost: 0.2, hallucination: 0.1."

**🤖 AI Agent:**
> AgentA: 0.82, AgentB: 0.78. Rank 1: AgentA, Rank 2: AgentB.

---

**👤 You:**
> "Who is the fastest agent among AgentX (latency: 500) and AgentY (latency: 200)?"

**🤖 AI Agent:**
> AgentY is the fastest agent with a latency of 200ms.

---

**👤 You:**
> "Check if these weights are valid: accuracy: 0.5, latency: 0.5."

**🤖 AI Agent:**
> The configuration is valid as the weights sum to 1.0.


## ❓ FAQ

**Q: How are the agent scores calculated?**
Scores are calculated by normalizing each metric to a 0.0-1.0 scale and applying user-defined weights to create a composite score.

**Q: Can I use custom weights for my evaluation?**
Yes, you can provide custom weights for accuracy, latency, cost, and hallucination rate using the `calculate_agent_rankings` tool, provided they sum to 1.0.

**Q: How do I ensure my configuration is valid?**
You can use the `validate_benchmark_config` tool to verify that your weights sum to 1.0 and all metrics are within logical bounds before running calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-benchmark-comparison-engine](https://vinkius.com/ai-agent-connect/agent-benchmark-comparison-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Benchmark Comparison Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-benchmark-comparison-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Benchmark Comparison Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-benchmark-comparison-engine": {
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
