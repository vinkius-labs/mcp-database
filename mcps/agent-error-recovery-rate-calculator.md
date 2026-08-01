# Agent Error Recovery Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agent-error-recovery-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyze execution logs to calculate error recovery rates and identify failure patterns.

## Description
The Agent Error Recovery Rate Calculator is a specialized MCP server designed for developers monitoring AI agent performance. By parsing execution logs in the format 'SUCCESS: ' or 'PREVIOUSLY FAILED:  - ', it calculates critical metrics like the recovery rate—the frequency of a successful tool call immediately following a failed one. The `analyze_logs` tool extracts exact error signatures such as 'SyntaxError' or 'Timeout', providing a clear view of how resilient your agentic workflows are to transient failures.


## Available Tools (1)
- **analyze_logs**: It will provide statistics on success, failure, and how often failures are recovered by subsequent successes.

Analyzes execution logs to calculate error recovery rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Error Recovery Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these logs: 'SUCCESS: tool_a', 'PREVIOUSLY FAILED: tool_b - Timeout', 'SUCCESS: tool_c'. What is the recovery rate?"

**🤖 AI Agent:**
> The recovery rate is 100.0% because one failure was immediately followed by a success.

---

**👤 You:**
> "Calculate the error signatures from these logs: 'PREVIOUSLY FAILED: tool_x - SyntaxError', 'PREVIOUSLY FAILED: tool_y - Timeout'."

**🤖 AI Agent:**
> The identified error signatures are: {"SyntaxError": 1, "Timeout": 1}.

---

**👤 You:**
> "Check the recovery rate for a log with 5 failures and 2 successes immediately following those failures."

**🤖 AI Agent:**
> The recovery rate is 40.0% (2 successes out of 5 failures).


## ❓ FAQ

**Q: What log format does the tool require?**
The `analyze_logs` tool expects logs in two specific formats: 'SUCCESS: <name>' for successful operations and 'PREVIOUSLY FAILED: <name> - <error>' to capture failures and their error signatures.

**Q: How is the recovery rate calculated?**
The recovery rate is computed by identifying every instance where a 'SUCCESS' entry immediately follows a 'PREVIOUSLY FAILED' entry, then dividing that count by the total number of failures.

**Q: Can it detect specific error types?**
Yes, the tool performs string matching to extract and count exact error signatures like 'Timeout', 'InvalidAPIKey', or 'SyntaxError' from your logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agent-error-recovery-rate-calculator](https://vinkius.com/mcp/agent-error-recovery-rate-calculator)
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
