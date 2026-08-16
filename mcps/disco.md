# DISCO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/disco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Query your DISCO eDiscovery datasets, data-usage changes, and review metrics directly from any AI agent via the official DISCO API.

## Description
Connect **DISCO**, the leading legal technology platform, to any AI agent through the official DISCO API. Query your eDiscovery **datasets**, track **data-usage changes** (ingest, deletion, volume deltas), and pull **review metrics** — including review-database sizes and names — using natural language.

### What you can do

- **Datasets** — List the datasets (matters) exposed to your API key, with optional name filtering.
- **Data-Usage Changes** — Audit the history of data-volume changes across your datasets.
- **Review Metrics** — Query review analytics, review-database sizes, and the list of available review-database names.

### How it works

1. Subscribe to this server.
2. Enter your **DISCO API Key** and **Organization ID** (from Organization Settings → API).
3. Make sure the MCP's egress IP is **CIDR-allowlisted** in your DISCO org settings (DISCO enforces IP allowlisting).
4. Query your discovery data and metrics through natural conversation.

### Who is this for?

- **Legal Operations** — Audit data usage and review-database sizes at a glance.
- **Litigation Support** — Track data ingest/deletion events across datasets.
- **Attorneys & Paralegals** — Surface review metrics during case planning.


## Available Tools (6)
- **get_data_usage_changes_metadata**: Retrieve the metadata schema for data-usage change events
- **get_metrics**: Pass a JSON payload to scope the query (e.g. metric name, date range, review-db filter).

Query review metrics from DISCO
- **get_reviewdb_size**: Pass an optional JSON payload to filter by review-db name or date.

Get the review database size metric
- **list_datasets**: Use the optional search to filter by name.

List datasets (matters) available in your DISCO organization
- **list_reviewdb_names**: List the names of available review databases
- **list_data_usage_changes**: g. ingest, deletion) across datasets.

List data-usage change events recorded for your datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DISCO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my datasets."

**🤖 AI Agent:**
> I've found your datasets exposed to the configured API key, including 'Smith vs. Jones' and 'Project Aurora Review'. Would you like to see the data-usage changes for the largest dataset?

---

**👤 You:**
> "What are the data-usage change events for this month?"

**🤖 AI Agent:**
> Here are the recent data-usage change events: two ingestions and one deletion across 'Project Aurora'. The total volume delta is +12.4 GB this month.

---

**👤 You:**
> "Show me the review-database sizes and names."

**🤖 AI Agent:**
> You have 3 review databases: 'Aurora-Review' (84 GB), 'Smith-Priv' (12 GB), and 'Acme-Merge' (6 GB). The 'list_reviewdb_names' tool returned the available names for scoping further queries.


## ❓ FAQ

**Q: How do I get DISCO API credentials?**
Log in to your DISCO account, navigate to Organization Settings → API, and copy your **API Key** and **Organization ID**. Both are required on every request (sent as the `disco-api-key` and `organization-id` headers).

**Q: Why are my requests returning 403 Access Denied?**
DISCO enforces CIDR block (IP allowlisting) verification per organization. You must add the MCP's egress IP address as a trusted source in Organization Settings → API, or every request will be rejected with 403 regardless of key correctness.

**Q: Can the agent download legal documents?**
No. The public DISCO API is read-only and exposes dataset, data-usage-change, and review-metric endpoints — not document content or downloads. Managing document content is done via the DISCO platform itself.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/disco](https://vinkius.com/ai-agent-connect/disco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DISCO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `disco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DISCO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disco": {
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
