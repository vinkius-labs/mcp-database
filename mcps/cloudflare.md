# Cloudflare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI edge infrastructure: manage Workers, KV, D1, R2, routes, and deployments via agents.

## Description
### What you can do

Connect AI agents to Cloudflare's platform for comprehensive edge infrastructure management:

- **Manage Workers** — list, inspect, delete serverless functions across your account
- **Control deployments** — version history, immediate/gradual rollouts, rollback capabilities
- **Manage secrets** — create, list, and delete encrypted environment secrets securely
- **Configure routes** — URL patterns that trigger Workers at specific paths or domains
- **Query KV storage** — read/write key-value pairs from Workers KV namespaces
- **Execute D1 queries** — run SQL queries against Cloudflare's serverless SQLite databases
- **Inspect R2 buckets** — list and manage object storage buckets
- **Monitor analytics** — zone traffic, Worker invocations, CPU usage, and error rates
- **Tail Worker logs** — create real-time logging sessions for debugging in production
- **Purge CDN cache** — clear cached content to serve fresh origin data

### How it works

1. **Generate a Cloudflare API token** with Workers, KV, D1, R2, and Analytics permissions
2. **Find your Account ID** from the Cloudflare dashboard
3. **Ask your AI agent** to deploy Workers, manage secrets, query databases, or monitor analytics
4. **Natural language commands** replace manual Wrangler CLI or dashboard operations

### Who is this for?

Essential for **edge application developers**, **serverless architects**, **DevOps engineers**, **full-stack developers**, and **platform teams** using Cloudflare's ecosystem. Let AI agents handle continuous Worker deployments, secret rotation, KV data management, D1 database queries, production debugging, and infrastructure monitoring. Perfect for teams running production workloads on Cloudflare who want to eliminate manual Wrangler steps, accelerate deployment cycles, and enable AI-driven edge operations.


## Available Tools
- **create_deployment**: Strategy can be immediate (100% traffic immediately) or gradual (percentage-based rollout). Requires script name, version ID, and deployment strategy. Use this to roll out new features, rollback to previous versions, or perform canary deployments.

Deploy a specific Worker version to traffic
- **create_secret**: Secrets are encrypted at rest and injected at runtime. Requires script name, secret name, and secret value. Common use: API keys, database passwords, OAuth tokens. The secret becomes available via env.VARIABLE_NAME in your Worker code.

Create or update a secret for a Cloudflare Worker
- **create_tail_session**: log() output and exceptions. Returns a tail ID and WebSocket URL for streaming logs. Use this for debugging Workers in production or monitoring error output.

Create a tail logging session for a Cloudflare Worker
- **create_worker_route**: Requires zone ID, URL pattern (e.g., "example.com/api/*"), and script name. Use this to expose your Worker at specific URL paths or domains.

Create a new route pattern for a Cloudflare Worker
- **delete_secret**: Use this to clean up unused secrets or rotate credentials. Requires script name and secret name. After deletion, the Worker will no longer have access to the secret value.

Delete a secret from a Cloudflare Worker
- **delete_tail_session**: Requires script name and tail ID. Use this to clean up unused tail sessions when debugging is complete.

Delete a tail logging session for a Cloudflare Worker
- **delete_worker_route**: Use this to stop serving a Worker at specific URLs. Requires zone ID and route ID.

Delete a route pattern from a Cloudflare Worker
- **delete_worker**: This action cannot be undone. Requires the script name. Confirm with the user before proceeding.

Delete a Cloudflare Worker script and all its associated resources
- **get_kv_key**: Returns the raw value as JSON. Use this to read configuration values, cached responses, or user data stored in KV.

Get the value of a specific key in a KV namespace
- **get_worker_analytics**: Returns data for recent invocations. Use this to monitor Worker performance, identify errors, or track usage trends.

Get analytics data for a specific Cloudflare Worker
- **get_worker**: Requires the script name from list_workers results. Use this to review Worker configuration before making updates or debugging.

Get detailed information about a specific Cloudflare Worker
- **get_worker_version**: Requires script name and version ID from list_worker_versions results. Use this to audit version contents or prepare for rollback deployment.

Get detailed information about a specific Worker version
- **get_zone_analytics**: Returns aggregated data for the last 24 hours. Use this to monitor traffic patterns, identify spikes, or measure CDN performance.

Get analytics data for a specific Cloudflare zone
- **list_d1_databases**: Returns database IDs, names, creation dates, and file sizes. Use this to identify available databases before querying.

List all D1 databases in your Cloudflare account
- **list_deployments**: Returns deployment IDs, version IDs, strategies (immediate, gradual), creation dates, and traffic percentages. Use this to review current deployment state, monitor gradual rollouts, or identify which version is live.

List all deployments for a specific Cloudflare Worker
- **list_kv_keys**: Returns key names, expiration metadata, and sizes. Use this to audit stored data or find specific keys before reading values.

List all keys in a specific KV namespace
- **list_kv_namespaces**: KV namespaces are key-value stores for Workers. Returns namespace IDs, titles, and creation dates. Use this to identify which namespaces exist before reading/writing data.

List all KV namespaces in your Cloudflare account
- **list_r2_buckets**: Returns bucket names, creation dates, and storage locations. Use this to identify available storage buckets before managing objects.

List all R2 storage buckets in your Cloudflare account
- **list_secrets**: Returns secret names and types (secret_text, secret_key). Secret values are never returned for security. Use this to audit which secrets are configured before adding new ones or cleaning up unused secrets.

List all secrets for a specific Cloudflare Worker
- **list_worker_routes**: Returns route patterns, associated script names, and zone IDs. Use this to understand which URLs invoke your Worker before adding or removing routes.

List all route patterns associated with a Cloudflare Worker
- **list_worker_versions**: Each version represents a deployed code snapshot with unique ID, creation date, and metadata. Returns version IDs, timestamps, and author information. Use this to review deployment history, rollback to previous versions, or audit code changes.

List all versions of a specific Cloudflare Worker
- **list_workers**: Returns script names, creation dates, modification dates, and deployment status. Use this as the first step to identify which Workers exist before managing versions, deployments, or secrets.

List all Cloudflare Workers scripts in your account
- **list_zones**: Returns zone IDs, domain names, status, plan, and name servers. Use this to identify zone IDs needed for Worker routes, DNS management, or cache operations.

List all DNS zones in your Cloudflare account
- **purge_cache**: Use this after deploying content changes or updating static assets. Requires zone ID.

Purge all cached content for a specific zone
- **query_d1**: Supports SELECT, INSERT, UPDATE, DELETE operations. Returns query results as JSON. Use this for data analysis, migrations, or ad-hoc queries. Requires database ID and SQL query string.

Execute a SQL query against a D1 database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudflare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all serverless Cloudflare Workers deployed natively bound to my account."

**🤖 AI Agent:**
> Pulling instances via `list_workers`. Extracting exactly 5 active edge-computation scripts securely operating on your endpoints mapping perfectly.

---

**👤 You:**
> "Query the KV namespace assigned to 'production_keys' and extract the specific text mapping 'gateway_url'."

**🤖 AI Agent:**
> Connecting KV namespaces natively... Resolved variable payload matching 'gateway_url': `api.vinkius.cloud` loaded efficiently without cache interference.

---

**👤 You:**
> "Check error statistics on my main D1 SQLite database instance over the last 24 hours."

**🤖 AI Agent:**
> Parsing telemetry array from metrics. The D1 metrics reveal stable instances with precisely 0% crash loops inside the isolated runtime edges.


## ❓ FAQ

**Q: Can I deploy new Worker scripts directly through the AI agent?**
Yes! You can orchestrate deployments natively mapping source code variables seamlessly without touching Wrangler.

**Q: Does it interact with specific D1 Serverless SQL definitions?**
Absolutely. Ask your agent to parse complex D1 databases and query tables instantly utilizing precise analytical calls.

**Q: How are environment variables and secrets handled?**
All `add_secret` queries execute symmetrically securely masking output variables while committing seamlessly inside Cloudflare matrices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare](https://vinkius.com/mcp/cloudflare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudflare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cloudflare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudflare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudflare": {
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
