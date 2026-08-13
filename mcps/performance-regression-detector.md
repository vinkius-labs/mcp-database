# Performance Regression Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/performance-regression-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Detects performance regressions and degradation trends in LLM agent execution times.

## Description
This MCP server provides statistical diagnostic tools to monitor LLM agent performance. It identifies execution time regressions using baseline medians and standard deviations, detects systematic degradation via linear regression trends, and predicts the time remaining before performance hits critical limits. Use `analyze_execution_performance` to find specific outliers, `detect_performance_trend` to see if speed is decreasing over time, and `predict_failure_horizon` to estimate when a performance threshold will be breached.


## Available Tools (3)
- **predict_failure_horizon**: Estimates how much longer the system can operate before execution times reach an unacceptable limit
- **analyze_execution_performance**: Identifies specific instances where execution time has deviated significantly from the established baseline
- **detect_performance_trend**: Determines if the agent's performance is systematically degrading over time using linear regression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Performance Regression Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if there are any performance regressions in these execution times: [10, 12, 11, 13, 25, 12, 11]."

**🤖 AI Agent:**
> Yes, a regression was detected. The execution time of 25 seconds exceeded the calculated threshold.

---

**👤 You:**
> "Is my agent's performance degrading based on these times: [5, 6, 7, 8, 9]?"

**🤖 AI Agent:**
> Yes, the performance is degrading with a positive trend slope indicating increasing execution times.

---

**👤 You:**
> "When will the execution time hit 20 seconds if the current trend continues for these times: [10, 11, 12]?"

**🤖 AI Agent:**
> Based on the current trend, the execution time is predicted to reach 20 seconds in approximately 8 more steps.


## ❓ FAQ

**Q: How is a performance regression defined?**
A regression is flagged when an execution time exceeds the baseline median plus two times the baseline standard deviation.

**Q: Can I predict when my agent will hit a performance limit?**
Yes, by using `predict_failure_horizon`, you can estimate the number of steps remaining before execution times reach a specified critical limit based on current trends.

**Q: What data is required for analysis?**
The tools require a chronological list of execution durations in seconds provided via the `executionTimeHistory` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/performance-regression-detector](https://vinkius.com/mcp/performance-regression-detector)
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
