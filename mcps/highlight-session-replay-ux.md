# Highlight (Session Replay & UX) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highlight-session-replay-ux)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/highlight-session-replay-ux-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/highlight-session-replay-ux-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Highlight (Session Replay & UX)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highlight-session-replay-ux](https://vinkius.com/mcp/highlight-session-replay-ux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
