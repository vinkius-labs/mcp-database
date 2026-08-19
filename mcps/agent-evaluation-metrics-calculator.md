# Agent Evaluation Metrics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-evaluation-metrics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic engine for measuring agentic performance through statistical accuracy, efficiency, and reliability metrics.

## Description
This MCP server provides a deterministic evaluation engine to quantify the performance of autonomous agents. It connects AI clients to specialized statistical tools that calculate core accuracy metrics like precision, recall, and F1 score. Users can analyze operational costs using `calculate_efficiency_and_latency` to track token and cost efficiency, or assess reliability with `calculate_calibration_error` to measure Expected Calibration Error (ECE). The engine also detects performance regressions by comparing current accuracy against established baselines using `calculate_performance_metrics`.


## Available Tools (3)
- **calculate_calibration_error**: Determines the Expected Calibration Error (ECE) to assess if the agent's confidence is trustworthy
- **calculate_efficiency_and_latency**: Analyzes the operational costs and temporal performance of the agent
- **calculate_performance_metrics**: Computes core statistical accuracy and reliability scores for a set of task results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Evaluation Metrics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the performance metrics for these results: [{"taskId": "1", "expectedOutput": "A", "actualOutput": "A", "latencyMs": 100, "tokensUsed": 50, "successBoolean": true, "confidenceScore": 0.9}]"

**🤖 AI Agent:**
> {"accuracy": 1.0, "precision": 1.0, "recall": 1.0, "f1Score": 1.0, "taskCompletionRate": 1.0, "isF1Low": false, "regressionDetected": false, "accuracyDropPercentage": 0.0}

---

**👤 You:**
> "What is the latency profile for these tasks: [{"taskId": "1", "latencyMs": 200, "tokensUsed": 100, "computeUnitsUsed": 10, "successBoolean": true}]"

**🤖 AI Agent:**
> {"averageLatency": 200, "p95Latency": 200, "tokenEfficiency": 0.01, "costEfficiency": 0.1}

---

**👤 You:**
> "Check the calibration error for these confidence scores: [{"confidenceScore": 0.8, "successBoolean": true}, {"confidenceScore": 0.8, "successBoolean": false}]"

**🤖 AI Agent:**
> {"expectedCalibrationError": 0.1, "calibrationStatus": "calibrated"}


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate accuracy, precision, recall, F1 score, task completion rate, average and p95 latency, token efficiency, cost efficiency, regression detection, and Expected Calibration Error (ECE).

**Q: How does the regression detection work?**
By using `calculate_performance_metrics`, you can provide a baseline accuracy. The tool will flag a regression if the current accuracy drops by more than 5% compared to that baseline.

**Q: Can I measure how much my agent costs to run?**
Yes, the `calculate_efficiency_and_latency` tool calculates cost efficiency by dividing the number of successful tasks by the total compute units used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-evaluation-metrics-calculator](https://vinkius.com/ai-agent-connect/agent-evaluation-metrics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Evaluation Metrics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-evaluation-metrics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Evaluation Metrics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-evaluation-metrics-calculator": {
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
