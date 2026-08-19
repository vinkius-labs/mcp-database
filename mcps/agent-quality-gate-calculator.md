# Agent Quality Gate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-quality-gate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

A deterministic engine for calculating quality scores, approval decisions, and operational costs for AI agent outputs.

## Description
This MCP server provides a deterministic engine to evaluate AI agent outputs against configurable quality criteria. It allows for precise gatekeeping using strategies like 'all_must_pass', 'majority_vote', or 'weighted_score'. Use `evaluate_output_quality` to determine if an output meets specific thresholds, `analyze_quality_trends` to monitor performance degradation over time, and `estimate_rework_impact` to calculate the business cost of inaccuracies. It is designed to help teams implement automated quality gates for various output types like code, summaries, or data extraction.


## Available Tools (3)
- **analyze_quality_trends**: Track the performance of an agent over time and identify patterns of degradation
- **estimate_rework_impact**: Calculate the business cost associated with agent inaccuracies
- **evaluate_output_quality**: Perform the core mathematical evaluation of a single agent output against a set of criteria and a strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Quality Gate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this JSON output for quality using the all_must_pass strategy with a threshold of 0.8."

**🤖 AI Agent:**
> The output has been evaluated. The composite quality score is 0.75, resulting in a decision of REJECT due to the format_validation score.

---

**👤 You:**
> "What is the estimated rework cost if my rejection rate is 0.15 and it takes 10 minutes to fix an error?"

**🤖 AI Agent:**
> The estimated rework cost is 1.5 minutes.

---

**👤 You:**
> "Analyze the quality trends for the last 50 outputs."

**🤖 AI Agent:**
> The rolling average is 0.88, the rejection rate is 0.05, and no performance decline was detected.


## ❓ FAQ

**Q: How does the gate decision work?**
The decision is determined by comparing the composite quality score against a provided threshold. If the score meets or exceeds the threshold, the decision is APPROVE; otherwise, it is REJECT.

**Q: What are the available gate strategies?**
The engine supports three strategies: 'all_must_pass' (the lowest score determines the result), 'majority_vote' (percentage of criteria passing a threshold), and 'weighted_score' (sum of weighted individual scores).

**Q: Can I track performance over time?**
Yes, you can use the `analyze_quality_trends` tool to monitor rolling averages, rejection rates, and detect if quality is declining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-quality-gate-calculator](https://vinkius.com/ai-agent-connect/agent-quality-gate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Quality Gate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-quality-gate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Quality Gate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-quality-gate-calculator": {
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
