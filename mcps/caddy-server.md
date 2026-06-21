# Caddy Server MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/caddy-server)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Caddy web server via API — update configurations, monitor upstreams, and handle PKI certificates directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caddy Server** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the full JSON configuration of my Caddy server."

**🤖 AI Agent:**
> I've retrieved the configuration. It contains 2 HTTP servers and 4 routes. Would you like me to analyze a specific path like 'apps/http'?

---

**👤 You:**
> "Adapt this Caddyfile to JSON: 'example.com { reverse_proxy localhost:8080 }'"

**🤖 AI Agent:**
> I've adapted the Caddyfile. The resulting JSON structure defines a server for 'example.com' with a reverse proxy handler pointing to 'localhost:8080'. Shall I apply this configuration using load_config?

---

**👤 You:**
> "Check the status of my proxy upstreams."

**🤖 AI Agent:**
> Fetching upstream status... I found 3 configured upstreams. All backends for 'api-cluster' are currently healthy, but one node in 'static-assets' is reporting a timeout. Would you like the full metrics?


## ❓ FAQ

**Q: Can I use a Caddyfile instead of JSON to update my configuration?**
Yes! Use the `load_config` tool and set the `content_type` to `text/caddyfile`. You can also use `adapt_config` to preview the JSON conversion before applying it.

**Q: How can I monitor the health of my load-balanced backends?**
Use the `get_upstreams` tool. It returns the current status and health metrics of all configured proxy upstreams in your Caddy instance.

**Q: Is it possible to remove a specific site or route without resetting the whole server?**
Absolutely. Use `delete_config` with the specific path (e.g., `apps/http/servers/srv0/routes/1`) to remove only that element from the active configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/caddy-server](https://vinkius.com/mcp/caddy-server)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caddy Server** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `caddy-server` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caddy Server** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caddy-server": {
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
