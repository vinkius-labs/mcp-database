# Typesense Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typesense-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate search cluster workflows via Typesense Cloud — monitor performance metrics, check cluster health, manage aliases, and execute multi-searches.

## Description
Connect your **Typesense Cloud** endpoint to any AI agent and take full control of your distributed lightning-fast search infrastructure natively through chat.

### What you can do

- **Cluster Lifecycle** — Verify the core operational reachability, checking if nodes are online and ingesting data uninterruptedly at high speed
- **Hardware Metrics** — Measure and fetch real-time latency thresholds, usage logs, active search workloads, and node resource consumption patterns
- **Federated Queries** — Issue sweeping multi-search commands across multiple targeted collections simultaneously sending raw JSON schemas securely
- **Aliasing & Key Mapping** — List virtual aliases abstracting concrete structures from public access, scaling robust API Key auditing natively

### How it works

1. Subscribe to this server
2. Enter both your active Typesense Host URL and API Key
3. Leverage your new infrastructure agent running globally from Claude, Cursor, or any MCP-compatible environment

No digging into terminal CURL outputs required to diagnose your search latency spikes. Delegate cluster forensics directly to a highly capable AI.

### Who is this for?

- **DevOps Professionals** — trigger on-the-spot node health interrogations, extracting metrics over latency peaks 
- **DBAs & Search Engineers** — validate multi-search endpoints logically before mapping onto the UI facing software
- **Sysadmins** — evaluate any lingering alias structures dynamically across test and production environments


## Available Tools (6)
- **get_cluster_health**: Checks the operational health status of the Typesense cluster
- **get_cluster_metrics**: Retrieves performance and usage metrics for the Typesense cluster
- **list_collection_aliases**: Lists all collection aliases (virtual names mapping to real collections)
- **list_collections**: Lists all search collections in the Typesense Cloud cluster
- **list_api_keys**: Lists all API keys configured for the Typesense cluster
- **execute_multi_search**: Provide a JSON array of search request objects.

Executes multiple search requests in a single API call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typesense Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the cluster health to verify Typesense is up in London."

**🤖 AI Agent:**
> The cluster responded successfully in 12ms. Status is 'ok'. Your Typesense nodes are fully operational.

---

**👤 You:**
> "List all active collections inside this database environment."

**🤖 AI Agent:**
> You have 3 core collections currently structured: 1. 'global_docs' (150,000 docs) 2. 'commerce_catalog' (2,000 docs) and 3. 'test_index_v1' (0 docs). Need the exact schema for the e-commerce one?

---

**👤 You:**
> "Fetch the performance metrics of the cluster and tell me if response times are above 100ms."

**🤖 AI Agent:**
> Pulling cluster metrics... The search_latency median is currently at 14ms globally. The 99th percentile spike reached 88ms. Fortunately, there are no endpoints dropping past 100ms. CPU stands at an idle 12% usage.


## ❓ FAQ

**Q: Can the AI provide an analysis if our search endpoints hit performance degradation?**
Yes. Instructing the agent to run the 'get_cluster_metrics' tool will pull out CPU times, active requests processing, and milliseconds threshold details so the AI inherently explains why the node slows down.

**Q: Can it execute a multi-search batch via chat?**
Absolutely. Give it a target array of searches (e.g., search product_A and product_B tables). It formats the payload perfectly to hit the endpoint natively and unpacks both search answers logically back to you.

**Q: Does it detect empty aliases mapped incorrectly?**
Yes! When listing all collections and matching them against 'list_aliases', the agent can see if a virtual layer points to a non-existent cluster data structure instantly. Very handy for debugging production releases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typesense-cloud](https://vinkius.com/mcp/typesense-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Typesense Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `typesense-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Typesense Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typesense-cloud": {
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
