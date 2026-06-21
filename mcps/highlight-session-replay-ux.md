# Highlight (Session Replay & UX) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highlight-session-replay-ux)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Streamline observability by ingesting raw logs, OTLP logs, and OTLP traces directly into Highlight for session replay and UX monitoring.

## Description
Connect your **Highlight** project to any AI agent to manage observability data and monitor user experiences through natural conversation.

### What you can do

- **Raw Log Ingestion** — Send text-based logs from backend services directly to your Highlight dashboard using the `ingest_raw_log` tool.
- **OTLP Log Support** — Ingest structured logs in OTLP JSON format to maintain rich context and metadata with `ingest_otlp_logs`.
- **Trace Management** — Send OTLP traces via `ingest_otlp_traces` to visualize request flows and identify performance bottlenecks.

### How it works

1. Subscribe to this server
2. Enter your Highlight Project ID
3. Start sending logs and traces from your development environment or AI agent.

### Who is this for?

- **Developers** — Quickly send logs from local environments to debug issues in the Highlight dashboard.
- **DevOps Engineers** — Automate the ingestion of structured OTLP data for better system visibility.
- **Product Managers** — Correlate backend logs with user sessions to understand UX friction points.


## Available Tools (3)
- **ingest_otlp_logs**: The payload must include the highlight.project_id attribute.

Ingest OTLP JSON logs into Highlight
- **ingest_otlp_traces**: Ingest OTLP JSON traces into Highlight
- **ingest_raw_log**: Ingest a raw log message into Highlight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Highlight (Session Replay & UX)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ingest a raw log message 'Server started' for the 'backend-api' service."

**🤖 AI Agent:**
> I've sent the raw log 'Server started' for 'backend-api' to your Highlight project. You can now view it in your dashboard.

---

**👤 You:**
> "Send this OTLP JSON log payload to Highlight: {"resourceLogs": [...]}."

**🤖 AI Agent:**
> Processing the OTLP logs... The structured payload has been successfully ingested into Highlight via `ingest_otlp_logs`.

---

**👤 You:**
> "Use ingest_otlp_traces to send these resource spans to Highlight."

**🤖 AI Agent:**
> The OTLP traces have been sent. You can now analyze the request spans and performance metrics in your Highlight project.


## ❓ FAQ

**Q: How can I send a basic text log message to my dashboard?**
You can use the `ingest_raw_log` tool. Simply provide the service name and the message content, and it will be sent directly to Highlight.

**Q: Does this server support structured OpenTelemetry logs?**
Yes! Use the `ingest_otlp_logs` tool to send structured logs in OTLP JSON format. Ensure your payload includes the project ID attribute.

**Q: Can I visualize request traces using this integration?**
Absolutely. The `ingest_otlp_traces` tool allows you to send OTLP JSON traces to Highlight, helping you track request spans and performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highlight-session-replay-ux](https://vinkius.com/mcp/highlight-session-replay-ux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Highlight (Session Replay & UX)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `highlight-session-replay-ux` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Highlight (Session Replay & UX)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "highlight-session-replay-ux": {
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
