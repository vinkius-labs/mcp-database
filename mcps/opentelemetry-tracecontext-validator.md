# OpenTelemetry TraceContext Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opentelemetry-tracecontext-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Validates W3C TraceContext and OpenTelemetry headers for distributed agent tracing.

## Description
The OpenTelemetry TraceContext Validator ensures your distributed traces remain unbroken across agent hops. By using tools like `validate_traceparent`, `validate_tracestate`, and `validate_full_context`, you can verify that traceparent and tracestate headers strictly adhere to W3C specifications. This prevents common observability failures caused by invalid versioning, incorrect hex lengths, or malformed key-value pairs in the tracing context.


## Available Tools (3)
- **validate_traceparent**: Validates a W3C TraceContext traceparent header
- **validate_tracestate**: Validates a W3C TraceContext tracestate header
- **validate_full_context**: Validates both traceparent and tracestate headers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTelemetry TraceContext Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this traceparent valid: 00-4bf92f3577b34da6a3ce949509f6a980-00f067aa0ba9021d-01?"

**🤖 AI Agent:**
> Yes, the traceparent is valid. The trace ID and parent ID are correctly formatted.

---

**👤 You:**
> "Check if this tracestate is correct: vendor1=value,vendor2=value"

**🤖 AI Agent:**
> The tracestate is valid and follows the key=value format.

---

**👤 You:**
> "Validate this context: traceparent=00-4bf92f3577b34da6a3ce949509f6a980-00f067aa0ba9021d-01, tracestate=mykey=myvalue"

**🤖 AI Agent:**
> The full context is valid. Both traceparent and tracestate headers meet W3C requirements.


## ❓ FAQ

**Q: What does `validate_traceparent` check?**
It verifies the version is '00', the trace-id is 32 hex characters, the parent-id is 16 hex characters, and flags are 2 hex characters.

**Q: How can I validate both headers at once?**
Use the `validate_full_context` tool to provide both traceparent and tracestate for a single, holistic validation check.

**Q: Does it support the `tracestate` header?**
Yes, the `validate_tracestate` tool checks for correct key=value formatting and ensures no member exceeds 256 characters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opentelemetry-tracecontext-validator](https://vinkius.com/mcp/opentelemetry-tracecontext-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTelemetry TraceContext Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opentelemetry-tracecontext-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTelemetry TraceContext Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opentelemetry-tracecontext-validator": {
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
