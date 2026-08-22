# Agent Evaluation Metrics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-evaluation-metrics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Quantify agent performance with deterministic accuracy, speed, and efficiency metrics.

## Description
This MCP server provides a deterministic engine to evaluate AI agent performance. It calculates core success metrics like accuracy, precision, recall, and F1 score using `calculate_core_metrics`. It also analyzes operational costs through `calculate_efficiency_metrics` to determine latency and token efficiency. Finally, it generates a weighted composite score and detects performance regressions via `calculate_composite_and_health` based on a defined baseline accuracy.


## Available Tools (3)
- **calculate_composite_and_health**: Generates a single performance score and determines if the agent is underperforming relative to a baseline
- **calculate_core_metrics**: Calculates the foundational performance indicators (accuracy, precision, recall, and F1 score) based on task outcomes
- **calculate_efficiency_metrics**: Analyzes the operational cost and speed of the agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Evaluation Metrics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the core metrics for these tasks: [{'task_id': '1', 'expected_output': 'A', 'actual_output': 'A', 'latency_ms': 100, 'tokens_used': 50, 'success_boolean': true}, {'task_id': '2', 'expected_output': 'B', 'actual_output': 'C', 'latency_ms': 150, 'tokens_used': 60, 'success_boolean': false}]"

**🤖 AI Agent:**
> {"accuracy": 0.5, "precision": 1.0, "recall": 0.5, "f1Score": 0.6666666666666666}

---

**👤 You:**
> "What is the token efficiency for 10 successful tasks using 500 tokens?"

**🤖 AI Agent:**
> 0.02

---

**👤 You:**
> "Check if an agent with 0.85 accuracy has regressed against a baseline of 0.95, with avg latency 200, efficiency 0.01, and weights {'accuracy_weight': 0.5, 'latency_weight': 0.3, 'efficiency_weight': 0.2}."

**🤖 AI Agent:**
> {"compositeScore": 0.505, "regressionFlag": true}


## ❓ FAQ

**Q: How do I calculate the F1 score?**
You can use the `calculate_core_metrics` tool by providing an array of task results. It will return the F1 score along with accuracy, precision, and recall.

**Q: What triggers a regression flag?**
A regression flag is triggered via `calculate_composite_and_health` if the current accuracy falls below 95% of your specified baseline accuracy.

**Q: How is token efficiency measured?**
Token efficiency is calculated by the `calculate_efficiency_metrics` tool as the ratio of successful tasks to the total number of tokens consumed.


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
