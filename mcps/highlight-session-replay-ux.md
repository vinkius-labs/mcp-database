# Highlight (Session Replay & UX) MCP Server

Streamline observability by ingesting raw logs, OTLP logs, and OTLP traces directly into Highlight for session replay and UX monitoring.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/highlight-session-replay-ux)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Highlight (Session Replay & UX)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highlight-session-replay-ux](https://vinkius.com/mcp/highlight-session-replay-ux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
