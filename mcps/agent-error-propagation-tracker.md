# Agent Error Propagation Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-error-propagation-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Trace error chains and calculate system impact in multi-agent environments.

## Description
This MCP server provides deterministic diagnostic capabilities for multi-agent systems. It identifies the origin of failures by tracing error flows through dependency chains and calculates critical impact metrics like blast radius and error amplification. Use `analyze_error_chain` to find the root cause of a failure sequence, `calculate_impact_metrics` to quantify the severity of an incident, and `evaluate_resilience` to assess how well your agents recover from cascading failures.


## Available Tools (3)
- **analyze_error_chain**: Identifies the specific sequence of errors forming a causal chain and finds the original culprit
- **calculate_impact_metrics**: Quantifies the severity and spread of an error event
- **evaluate_resilience**: Determines how well agents recover from failures and how many are failing due to cascades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Error Propagation Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these error logs to find the root cause and the error chain."

**🤖 AI Agent:**
> The root cause was Agent-A. The error chain is: Agent-A (Timeout) -> Agent-B (Dependency Failure) -> Agent-C (Service Unavailable).

---

**👤 You:**
> "Calculate the impact of the recent failures using a 60 second window."

**🤖 AI Agent:**
> The incident resulted in 4 correlated errors and consumed 20% of your error budget.

---

**👤 You:**
> "Check the resilience of my agents after the last cascade."

**🤖 AI Agent:**
> The system detected a cascading failure, but the retry success rate for Agent-B was 100%.


## ❓ FAQ

**Q: How does the tool identify the root cause?**
The `analyze_error_chain` tool traverses the dependency graph alongside error timestamps to find the first agent in a causal sequence that failed.

**Q: What is a blast radius?**
The blast radius is the total count of unique agents negatively impacted by a specific failure sequence.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-error-propagation-tracker](https://vinkius.com/ai-agent-connect/agent-error-propagation-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Error Propagation Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-error-propagation-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Error Propagation Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-error-propagation-tracker": {
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
