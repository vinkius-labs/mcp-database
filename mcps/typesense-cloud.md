# Typesense Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typesense-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/typesense-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/typesense-cloud-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Typesense Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typesense-cloud](https://vinkius.com/mcp/typesense-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
