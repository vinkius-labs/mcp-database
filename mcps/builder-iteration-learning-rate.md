# Builder Iteration Learning Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/builder-iteration-learning-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyzes learning velocity and execution efficiency in iterative development cycles.

## Description
This MCP server provides a specialized analytical engine to measure how effectively a builder converts iterative cycles into actionable knowledge and execution velocity. By utilizing tools like `get_learning_rate_score` and `get_iteration_efficiency_audit`, it calculates the efficiency of the learning loop, identifies improvement trajectories, and recommends an optimal iteration cadence. It helps identify if a process is accelerating, stalling, or churning based on implementation rates and pivot frequency.


## Available Tools (4)
- **get_improvement_trajectory**: Determines the momentum and direction of the builder's learning progress over time
- **get_iteration_efficiency_audit**: Provides a diagnostic overview by combining all metrics to identify if the builder is churning or stalling
- **get_learning_rate_score**: Calculates the primary efficiency metric for a builder's current iteration cycle
- **get_optimal_cadence**: Recommends the ideal frequency for future iterations to maximize efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder Iteration Learning Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my current learning rate score with 10 iterations, 5 learnings per iteration, 80% implementation, and 2 pivots."

**🤖 AI Agent:**
> Your current learning rate score is 7.2, indicating a highly efficient and stable learning loop.

---

**👤 You:**
> "Check my efficiency status for 5 iterations, 2 learnings per iteration, 90% implementation, and 4 pivots."

**🤖 AI Agent:**
> Your efficiency status is 'Churning' due to a high pivot frequency relative to your implementation rate.

---

**👤 You:**
> "What is my improvement trajectory given these historical scores: 5.0, 5.5, 6.0?"

**🤖 AI Agent:**
> Your trajectory shows an accelerating trend with a positive velocity, indicating increasing efficiency over time.


## ❓ FAQ

**Q: What is the Learning Rate Score?**
The Learning Rate Score is a normalized metric that represents the efficiency of your iteration loop by combining knowledge gain with implementation speed.

**Q: How can I identify if my process is stalling?**
You can use the `get_iteration_efficiency_audit` tool. Stalling is typically identified when the implementation rate is high but the number of learnings per iteration is near zero.

**Q: What does the optimal cadence recommendation mean?**
The `get_optimal_cadence` tool suggests the ideal frequency for future cycles. For example, if pivot frequency is high, it may suggest a longer interval to ensure stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/builder-iteration-learning-rate](https://vinkius.com/ai-agent-connect/builder-iteration-learning-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Builder Iteration Learning Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `builder-iteration-learning-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Builder Iteration Learning Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "builder-iteration-learning-rate": {
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
