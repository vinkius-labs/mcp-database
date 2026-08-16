# Performance Regression Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/performance-regression-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Detects performance regressions and predicts execution time failures in LLM workflows.

## Description
This MCP server identifies performance regressions in agent execution times to prevent cost spikes and reliability degradation. It uses deterministic statistical calculations to identify anomalies via `analyze_execution_anomalies`, determine systemic slowdowns with `calculate_performance_trend`, and forecast future latency breaches using `predict_failure_horizon`.


## Available Tools (3)
- **predict_failure_horizon**: Forecasts when performance will reach a critical limit based on current degradation trends
- **analyze_execution_anomalies**: Identifies specific execution instances that deviate significantly from historical performance
- **calculate_performance_trend**: Determines if the system is experiencing a systemic slowdown over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Performance Regression Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any performance regressions in my recent execution history?"

**🤖 AI Agent:**
> Yes, there is a regression detected. The recent execution time exceeded the threshold of 1.5s.

---

**👤 You:**
> "Is my agent's performance degrading over time?"

**🤖 AI Agent:**
> Yes, the trend slope is positive, indicating a systemic slowdown in execution times.

---

**👤 You:**
> "How many cycles until we hit a 5-second latency limit?"

**🤖 AI Agent:**
> Based on the current degradation trend, there are approximately 12 execution cycles remaining before the 5-second limit is reached.


## ❓ FAQ

**Q: How does the tool identify a regression?**
An execution is flagged as a regression if its duration exceeds the baseline median plus two times the baseline standard deviation.

**Q: Can I predict when my agent will hit a latency limit?**
Yes, by using `predict_failure_horizon`, you can estimate the number of execution cycles remaining before a critical latency limit is breached based on current trends.

**Q: What is the purpose of the trend analysis?**
The `calculate_performance_trend` tool uses linear regression to determine if the system is experiencing a systemic slowdown over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/performance-regression-detector](https://vinkius.com/ai-agent-connect/performance-regression-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Performance Regression Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `performance-regression-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Performance Regression Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "performance-regression-detector": {
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
