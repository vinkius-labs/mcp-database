# Execution Trace Recorder and Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/execution-trace-recorder-and-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Records and validates agent execution traces to ensure integrity, determinism, and performance.

## Description
This MCP server provides essential diagnostic tools to solve the 'black box' problem in agentic workflows. It allows AI agents to record discrete execution events using `record_trace_step` and verify the continuity of their workflows. By using `validate_trace_integrity`, agents can ensure that the output of one step correctly feeds into the next via hash matching. Additionally, `detect_anomalies` identifies non-deterministic behavior and latency outliers, ensuring your agentic chains remain reliable and performant. Connect via Vinkius Edge to integrate these diagnostic capabilities into Cursor, Claude Desktop, VS Code, or Windsurf.


## Available Tools (3)
- **detect_anomalies**: Analyzes a trace to find non-deterministic behavior and significant timing outliers
- **record_trace_step**: Records a single discrete execution event within an agent's lifecycle
- **validate_trace_integrity**: Checks a collection of recorded steps to ensure the chain is unbroken and logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Execution Trace Recorder and Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the integrity of this execution trace: [{"agentId": "agent-1", "actionType": "thought", "inputHash": "h1", "outputHash": "h2", "timestampMs": 1700000000000, "durationMs": 500}]"

**🤖 AI Agent:**
> {"isTraceValid": true, "anomalyList": [], "stepCount": 1, "totalDurationMs": 500}

---

**👤 You:**
> "Check for anomalies in this trace sequence."

**🤖 AI Agent:**
> {"isTraceValid": false, "anomalyList": ["Latency anomaly at step 2"], "stepCount": 2, "totalDurationMs": 1500}

---

**👤 You:**
> "Record a new execution step for agent 'executor-01'."

**🤖 AI Agent:**
> {"agentId": "executor-01", "actionType": "tool_call", "inputHash": "abc", "outputHash": "def", "timestampMs": 1700000001000, "durationMs": 250}


## ❓ FAQ

**Q: How does this tool ensure trace integrity?**
It uses `validate_trace_integrity` to verify that the output hash of one step matches the input hash of the subsequent step, ensuring a continuous and unbroken chain.

**Q: What is a determinism anomaly?**
A determinism anomaly occurs when the same input hash results in different output hashes across different steps, which can be detected using `detect_anomalies`.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP server to Claude Desktop, Cursor, VS Code, and other compatible clients via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/execution-trace-recorder-and-validator](https://vinkius.com/ai-agent-connect/execution-trace-recorder-and-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Execution Trace Recorder and Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `execution-trace-recorder-and-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Execution Trace Recorder and Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "execution-trace-recorder-and-validator": {
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
