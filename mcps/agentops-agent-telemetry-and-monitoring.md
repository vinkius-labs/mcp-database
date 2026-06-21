# AgentOps (Agent Telemetry and Monitoring) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agentops-agent-telemetry-and-monitoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor and observe your AI agents with AgentOps — track traces, spans, and project metrics directly from your agent.

## Description
Connect **AgentOps** to your AI agent for comprehensive telemetry and observability of your agentic workflows. Gain deep insights into how your agents perform, identify bottlenecks, and track costs in real-time.

### What you can do

- **Project Insights** — Retrieve high-level details about your current AgentOps project associated with your API key using `get_project`.
- **Trace Analysis** — Inspect specific execution traces with `get_trace` to understand agent behavior, decision-making, and flow.
- **Cost & Token Monitoring** — Use `get_trace_metrics` to get detailed metrics for specific traces, including token usage counts and associated costs.
- **Granular Span Inspection** — Drill down into individual spans within a trace using `get_span` for deep debugging of specific tool calls or LLM interactions.

### How it works

1. Subscribe to this server
2. Enter your AgentOps API Key
3. Start monitoring your agent's performance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — Debug complex agentic loops and identify exactly where a process failed or slowed down.
- **Product Managers** — Monitor token costs and usage patterns across agent deployments to optimize ROI.
- **DevOps Teams** — Ensure the reliability and observability of production AI agents with structured telemetry data.


## Available Tools
- **get_trace**: Get details for a specific trace
- **get_project**: Get AgentOps project details
- **get_span**: Get details for a specific span
- **get_trace_metrics**: Get metrics for a specific trace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AgentOps (Agent Telemetry and Monitoring)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the details for my current AgentOps project."

**🤖 AI Agent:**
> I've retrieved your project details. Your current project is 'Production-Agent-v2' (ID: ao_proj_882). It is currently active and receiving telemetry data.

---

**👤 You:**
> "Show me the metrics and token costs for trace ID trace_abc123."

**🤖 AI Agent:**
> For trace trace_abc123, the total token count was 1,450 (800 prompt, 650 completion) with an estimated cost of $0.028. The execution took 4.2 seconds across 5 spans.

---

**👤 You:**
> "Inspect the details of span ID span_998877."

**🤖 AI Agent:**
> Span span_998877 was a 'tool_call' to 'web_search'. It started at 10:05:02 and finished at 10:05:04. Input parameters included 'query: agent observability' and it returned 3 search results.


## ❓ FAQ

**Q: How can I check the token usage and cost for a specific agent execution?**
You can use the `get_trace_metrics` tool by providing the specific Trace ID. It will return detailed data on token counts and the calculated financial cost for that execution.

**Q: Can I see the details of a single step within a larger trace?**
Yes! Use the `get_span` tool with the specific Span ID. This allows you to isolate and inspect individual operations, such as a single tool call or a specific LLM completion.

**Q: How do I verify which AgentOps project is currently active?**
Simply run the `get_project` tool. It retrieves the metadata and configuration details of the project associated with your current API key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agentops-agent-telemetry-and-monitoring](https://vinkius.com/mcp/agentops-agent-telemetry-and-monitoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AgentOps (Agent Telemetry and Monitoring)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `agentops-agent-telemetry-and-monitoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AgentOps (Agent Telemetry and Monitoring)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agentops-agent-telemetry-and-monitoring": {
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
