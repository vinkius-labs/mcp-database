# Prometheus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prometheus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor your infrastructure with Prometheus — run PromQL queries, analyze metrics, and manage time-series data directly from your AI agent.

## Description
Connect your **Prometheus** instance to any AI agent and transform your observability data into actionable insights through natural conversation.

### What you can do

- **Instant & Range Queries** — Evaluate complex PromQL expressions for real-time status or historical trends over specific time windows.
- **Metric Discovery** — Find time series matching specific label selectors and explore available labels and their values across your environment.
- **Metadata Inspection** — Retrieve detailed metadata about metrics scraped from targets to understand units, types, and help text.
- **Admin Operations** — Create data snapshots, delete specific series, and clean tombstones (requires admin API enabled).
- **System Status** — Inspect your Prometheus configuration, flags, and runtime information to ensure your monitoring stack is healthy.

### How it works

1. Subscribe to this server
2. Enter your Prometheus Server URL (and optional Auth Token)
3. Start querying your metrics from Claude, Cursor, or any MCP-compatible client

No more manual dashboard building just to answer a quick question about system health. Your AI acts as a dedicated SRE or DevOps engineer.

### Who is this for?

- **SRE & DevOps Engineers** — instantly troubleshoot incidents by querying metrics and checking configurations without leaving the terminal or chat.
- **Backend Developers** — verify service performance and resource consumption directly from the code editor.
- **Platform Teams** — automate infrastructure health reports and audit monitoring configurations via natural language.


## Available Tools (14)
- **get_status_config**: Get the currently loaded Prometheus configuration (YAML)
- **get_status_flags**: Get configured Prometheus flag values
- **get_status_runtimeinfo**: Get Prometheus runtime information
- **get_status_tsdb**: Get TSDB cardinality statistics
- **get_label_values**: Get all values for a specific label
- **get_labels**: Get a list of all label names
- **get_metadata**: Get metadata about metrics scraped from targets
- **query_range**: Evaluate a PromQL expression over a range of time
- **query**: Evaluate a PromQL expression at a single point in time
- **find_series**: Find time series matching label selectors
- **create_snapshot**: enable-admin-api to be enabled on the Prometheus server.

Create a snapshot of all current data
- **get_status_buildinfo**: Get Prometheus build information
- **clean_tombstones**: enable-admin-api to be enabled.

Remove deleted data from disk
- **delete_series**: enable-admin-api to be enabled.

Delete data for a selection of series in a time range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prometheus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run an instant query for 'up' to see which targets are currently reachable."

**🤖 AI Agent:**
> I've executed the `query`. All 5 targets are currently returning a value of 1, meaning they are all 'up' and healthy.

---

**👤 You:**
> "Show me the average CPU usage for the last 30 minutes using query_range."

**🤖 AI Agent:**
> I've fetched the range data. The average CPU usage across your nodes peaked at 45% about 10 minutes ago and has since stabilized at 20%.

---

**👤 You:**
> "What is the metadata for the metric 'http_requests_total'?"

**🤖 AI Agent:**
> Using `get_metadata`, I found that 'http_requests_total' is a Counter metric. It tracks the total number of HTTP requests received, partitioned by status code and method.


## ❓ FAQ

**Q: Can I run a PromQL query to get the current value of a metric?**
Yes. Use the `query` tool to evaluate any PromQL expression at a single point in time. This is perfect for checking current CPU usage, memory levels, or error rates.

**Q: How do I see how a metric has changed over the last hour?**
Use the `query_range` tool. You can specify the `start` and `end` timestamps along with a `step` duration to retrieve historical data points for graphing or trend analysis.

**Q: Can I perform administrative tasks like creating backups?**
Yes, if your Prometheus server has the Admin API enabled (`--web.enable-admin-api`), you can use the `create_snapshot` tool to create a snapshot of all current data on disk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prometheus](https://vinkius.com/mcp/prometheus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prometheus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prometheus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prometheus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prometheus": {
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
