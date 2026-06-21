# Logflare (Log Management Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/logflare-log-management-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/logflare-log-management-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/logflare-log-management-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Streamline log management and analytics via Logflare — ingest events, execute ad-hoc SQL queries, and trigger pre-configured endpoints directly from your AI agent.

## Description
Connect your **Logflare** account to any AI agent to monitor, analyze, and manage your log data through natural language. Logflare provides a powerful interface for BigQuery-backed log storage and retrieval.

### What you can do

- **Log Ingestion** — Send batches of log events to specific sources using either their unique UUID or human-readable name.
- **Ad-hoc SQL Queries** — Execute complex BigQuery or PostgreSQL queries against your log data to find patterns or troubleshoot issues.
- **Endpoint Execution** — Trigger pre-configured Logflare Endpoints with custom parameters to retrieve structured analytical reports.
- **Real-time Monitoring** — Query your logs instantly to get the latest status of your applications and infrastructure.

### How it works

1. Subscribe to this server
2. Enter your Logflare Access Token (API Key)
3. Start analyzing your logs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly query logs to identify the root cause of production incidents without leaving the terminal or chat.
- **Data Analysts** — run SQL queries against log data to generate usage reports or performance metrics.
- **Backend Developers** — ingest custom application logs during testing or debugging phases to monitor flow in real-time.


## Available Tools
- **ingest_logs_by_id**: Requires ingest scope.

Ingest log events into a Logflare source by UUID
- **ingest_logs_by_name**: Requires ingest scope.

Ingest log events into a Logflare source by Name
- **management_query**: Requires management scope. Must include a WHERE filter on the timestamp field.

Execute an ad-hoc SQL query against Logflare
- **query_endpoint_by_id**: Pass interpolation parameters as a JSON object.

Query a Logflare Endpoint by UUID
- **query_endpoint_by_name**: Pass interpolation parameters as a JSON object.

Query a Logflare Endpoint by Name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Logflare (Log Management Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a log to 'api-logs' saying 'Connection timeout' with metadata {'service': 'auth'}."

**🤖 AI Agent:**
> I've successfully ingested the log event into the 'api-logs' source using `ingest_logs_by_name`. The event is now available for analysis.

---

**👤 You:**
> "Run a SQL query to find the top 5 IP addresses from the 'web-traffic' source in the last hour."

**🤖 AI Agent:**
> I've executed the `management_query`. Here are the top 5 IP addresses found: [List of IPs]. I included the required timestamp filter for the last 60 minutes.

---

**👤 You:**
> "Query the endpoint 'daily-summary' with the parameter 'date' set to '2023-10-27'."

**🤖 AI Agent:**
> I've retrieved the data from the 'daily-summary' endpoint using `query_endpoint_by_name`. The summary for that date shows 15,420 total events.


## Installation & Usage

To install and use the **Logflare (Log Management Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logflare-log-management-analytics](https://vinkius.com/mcp/logflare-log-management-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
