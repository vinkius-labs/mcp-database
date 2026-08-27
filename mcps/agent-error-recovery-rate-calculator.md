# Agent Error Recovery Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-error-recovery-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyzes execution logs to calculate tool call success ratios and agent recovery rates.

## Description
This MCP server provides specialized tools to analyze the resilience of AI agents by parsing execution logs. It identifies specific error signatures and computes critical performance metrics, such as the success-to-failure ratio and the recovery rate. Use `parse_execution_logs` to structure raw logs, `calculate_error_distribution` to identify error patterns, and `calculate_resilience_metrics` to determine how effectively an agent recovers from failures.


## Available Tools (3)
- **calculate_error_distribution**: Provides a breakdown of how many times specific errors occurred
- **parse_execution_logs**: Extracts a structured sequence of tool call outcomes and error types from raw text logs
- **calculate_resilience_metrics**: Computes the high-level performance ratios regarding reliability and recovery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Error Recovery Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you analyze these logs and tell me the recovery rate?"

**🤖 AI Agent:**
> The recovery rate for the provided logs is 75%, meaning 3 out of 4 failures were followed by a successful tool call.

---

**👤 You:**
> "What are the most common errors in my execution history?"

**🤖 AI Agent:**
> The most frequent error identified is 'Timeout', which occurred 5 times in the analyzed logs.

---

**👤 You:**
> "Parse these logs for me."

**🤖 AI Agent:**
> I have parsed the logs. I found 10 total events: 8 successes and 2 failures.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can calculate the success-to-failure ratio and the recovery rate percentage using `calculate_resilience_metrics` after parsing your logs.

**Q: How do I start analyzing my logs?**
Start by using `parse_execution_logs` to convert your raw text logs into a structured format that the other tools can process.

**Q: What is a recovery rate?**
The recovery rate is the percentage of tool call failures that are immediately followed by a successful tool call, indicating the agent's ability to self-correct.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-error-recovery-rate-calculator](https://vinkius.com/ai-agent-connect/agent-error-recovery-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Error Recovery Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-error-recovery-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Error Recovery Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-error-recovery-rate-calculator": {
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
