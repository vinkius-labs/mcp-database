# OpenTelemetry Trace Latency Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opentelemetry-trace-latency-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Analyze OpenTelemetry traces to identify latency bottlenecks and critical path inefficiencies.

## Description
This MCP server provides a diagnostic engine for deconstructing OpenTelemetry-style traces. By analyzing spans with start/end timestamps and parent-child relationships, it computes critical-path duration, per-span self-time (excluding children), span-count and depth per trace, longest-chain bottleneck identification, and percentage of total trace duration attributable to each service or span-name group. Use `analyze_trace_latency` for high-level metrics, `identify_bottlenecks` to find slow spans, and `get_service_distribution` to see latency distribution across services.


## Available Tools (3)
- **get_service_distribution**: Calculate average latency per service/span name
- **analyze_trace_latency**: Analyze trace spans for latency metrics
- **identify_bottlenecks**: Identify spans that exceed a latency threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTelemetry Trace Latency Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this trace for latency: [{"id": "1", "parentID": null, "serviceName": "gateway", "spanName": "entry", "start": 1000, "end": 2000}, {"id": "2", "parentID": "1", "serviceName": "auth", "spanName": "validate", "start": 1100, "end": 1500}]"

**🤖 AI Agent:**
> The trace analysis shows a total duration of 1000ms. The gateway entry span has an average latency of 1000ms, while the auth validation span contributes 400ms.

---

**👤 You:**
> "Identify bottlenecks in this trace where spans exceed 50ms: [{"id": "1", "parentID": null, "serviceName": "api", "spanName": "root", "start": 0, "end": 200}, {"id": "2", "parentID": "1", "serviceName": "db", "spanName": "query", "start": 10, "end": 150}]"

**🤖 AI Agent:**
> The following bottleneck was identified: the `db` service span `query` contributed 140ms of self-time, exceeding your 50ms threshold.

---

**👤 You:**
> "What is the latency distribution for these spans?"

**🤖 AI Agent:**
> The service distribution shows that 'auth-service' has an average latency of 45ms and 'payment-service' has an average latency of 120ms.


## ❓ FAQ

**Q: What kind of trace data does this tool support?**
It supports OpenTelemetry-style traces where each span includes a unique identifier, parent ID, service name, span name, and start/end timestamps.

**Q: How can I identify the slowest parts of my request?**
By using `identify_bottlenecks`, you can find spans that exceed a specific latency threshold within your trace data.

**Q: Can I see how much time each service contributes to the total trace?**
Yes, using `get_service_distribution` allows you to see an aggregation of average latency per service or span name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opentelemetry-trace-latency-analyzer](https://vinkius.com/mcp/opentelemetry-trace-latency-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTelemetry Trace Latency Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opentelemetry-trace-latency-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTelemetry Trace Latency Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opentelemetry-trace-latency-analyzer": {
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
