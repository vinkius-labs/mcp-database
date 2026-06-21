# Prometheus MCP Server

Monitor your infrastructure with Prometheus — run PromQL queries, analyze metrics, and manage time-series data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/prometheus)

## Overview
**Category:** loved-by-devs
**Tools Count:** 14

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


## Available Tools
- **clean_tombstones**: enable-admin-api to be enabled.

Remove deleted data from disk
- **delete_series**: enable-admin-api to be enabled.

Delete data for a selection of series in a time range
- **get_label_values**: Get all values for a specific label
- **get_labels**: Get a list of all label names
- **get_metadata**: Get metadata about metrics scraped from targets
- **query_range**: Evaluate a PromQL expression over a range of time
- **query**: Evaluate a PromQL expression at a single point in time
- **find_series**: Find time series matching label selectors
- **create_snapshot**: enable-admin-api to be enabled on the Prometheus server.

Create a snapshot of all current data
- **get_status_buildinfo**: Get Prometheus build information
- **get_status_config**: Get the currently loaded Prometheus configuration (YAML)
- **get_status_flags**: Get configured Prometheus flag values
- **get_status_runtimeinfo**: Get Prometheus runtime information
- **get_status_tsdb**: Get TSDB cardinality statistics


## Installation & Usage

To install and use the **Prometheus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prometheus](https://vinkius.com/mcp/prometheus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
