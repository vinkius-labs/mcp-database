# OpenTelemetry Trace Context Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opentelemetry-trace-context-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Extracts W3C TraceContext fields from HTTP headers.

## Description
The OpenTelemetry Trace Context Extractor solves the observability problem of broken traces across agent hops. By using the `extract_trace_context` tool, you can provide a W3C TraceContext traceparent header and receive precisely parsed fields including trace ID, parent ID, and trace flags. The extractor uses strict regex validation (version-traceid-parentid-flags) and V8 string splitting to ensure deterministic results, verifying that the trace ID is a valid 3arget 32 hex characters and not all zeros.


## Available Tools (1)
- **extract_trace_context**: extractor for W3C TraceContext fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTelemetry Trace Context Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract context from this header: 00-4bf92f3577b34da6a3ce97d607f97781-00f067aa0ba902b7-01"

**🤖 AI Agent:**
> The extracted trace context is: Trace ID: 4bf92f3577b34da6a3ce97d607f97781, Parent ID: 00f067aa0ba902ds7, Flags: 01.

---

**👤 You:**
> "Validate this traceparent header: 00-invalid-header-01"

**🤖 AI Agent:**
> The header is invalid because the trace ID does not meet the required 32 hex character format.

---

**👤 You:**
> "What are the flags in this header: 00-4bf92f3577b34da6a3ce97d607f97781-00f067aa0ba902b7-00"

**🤖 AI Agent:**
> The trace flags for this header are 00.


## ❓ FAQ

**Q: What does this tool extract?**
It extracts the trace ID, parent ID, and trace flags from a W3C TraceContext `traceparent_header`.

**Q: How does it validate the header?**
It uses a strict RegExp pattern (version-traceid-parentid-flags) and verifies that the trace ID is 32 hex characters and not all zeros.

**Q: Is it compatible with standard W3C headers?**
Yes, it is specifically designed to parse the `traceparent` header following the W3C TraceContext specification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opentelemetry-trace-context-extractor](https://vinkius.com/mcp/opentelemetry-trace-context-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTelemetry Trace Context Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opentelemetry-trace-context-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTelemetry Trace Context Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opentelemetry-trace-context-extractor": {
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
