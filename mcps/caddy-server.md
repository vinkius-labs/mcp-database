# Caddy Server MCP Server

Manage your Caddy web server via API — update configurations, monitor upstreams, and handle PKI certificates directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/caddy-server)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect your **Caddy Server** instance to any AI agent and automate your web infrastructure management through natural conversation.

### What you can do

- **Configuration Management** — Load, get, append, or replace server configurations using JSON or Caddyfile formats.
- **Caddyfile Adaptation** — Instantly convert Caddyfile text into native Caddy JSON without applying the changes.
- **Upstream Monitoring** — Check the real-time status and health of your proxy upstreams and backends.
- **PKI & Certificates** — Inspect internal CA information and retrieve certificate chains for your managed domains.
- **Metrics & Observability** — Access Prometheus-style metrics to monitor server performance and request traffic.
- **Granular Control** — Delete specific configuration paths or gracefully stop the server process.

### How it works

1. Subscribe to this server
2. Enter your Caddy Admin API URL (e.g., http://localhost:2019)
3. Start managing your reverse proxies and web servers from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — automate infrastructure updates and monitor backend health without leaving the terminal or chat.
- **Web Developers** — quickly test and adapt Caddyfile configurations during local development.
- **SREs** — retrieve live metrics and PKI status to ensure site reliability and security compliance.


## Available Tools
- **adapt_config**: Adapts a configuration (e.g., Caddyfile) to JSON without running it
- **append_config**: and target is array, expands payload array and appends elements.

Sets or replaces an object; appends to an array in Caddy config
- **delete_config**: Deletes the value at the named path in Caddy config
- **get_config_by_id**: Access a configuration object directly via its @id field
- **get_config**: Leave empty for full config.

Exports the configuration at the specified path as JSON
- **get_metrics**: Exposes metrics in Prometheus exposition format
- **get_pki_ca_certs**: Returns the certificate chain for a particular CA
- **get_pki_ca**: Returns information about a particular PKI app CA
- **get_upstreams**: Returns the current status of configured proxy upstreams
- **insert_config**: Creates a new object or inserts into an array at a specific index
- **load_config**: Use application/json for native JSON, or text/caddyfile for Caddyfile.

Sets or replaces the active Caddy configuration
- **replace_config**: Strictly replaces an existing object or array element in Caddy config
- **stop_server**: Gracefully shuts down the Caddy server and exits the process


## Installation & Usage

To install and use the **Caddy Server** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/caddy-server](https://vinkius.com/mcp/caddy-server)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
