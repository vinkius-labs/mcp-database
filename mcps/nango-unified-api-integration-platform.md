# Nango (Unified API & Integration Platform) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nango-unified-api-integration-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nango-unified-api-integration-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nango-unified-api-integration-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Manage product integrations via Nango — audit OAuth connections, track data syncs, and explore unified records.

## Description
Connect your **Nango** account to any AI agent and take full control of your product's integrations, OAuth connections, and automated data synchronization through natural conversation.

### What you can do

- **Integration Orchestration** — List all configured integration logics across 700+ providers and retrieve detailed sync parameters and provider keys directly from your agent
- **Connection Management** — List and audit authenticated OAuth or credential-based connections to verify which customers have linked which external platforms securely
- **Sync Monitoring** — Track the real-time status and historical logs of automated data synchronizations to identify processing errors or data drift natively
- **Unified Record Access** — Explore actual synchronized data records for specific models (e.g., contacts, deals, tasks) across your entire connection pool securely
- **Credential Audit** — Retrieve precise metadata mapping authentication payloads and token boundaries for any specific Nango connection instantly
- **Environment Visibility** — Inspect your environment's runtime mapping logic and host constraints to ensure your integration infrastructure is healthy and correctly configured

### How it works

1. Subscribe to this server
2. Enter your Nango Secret Key
3. Start managing your integrations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — audit customer connection health and verify integration statuses through natural conversation without manual dashboard navigation
- **Software Developers** — test data sync logic and verify unified record schemas across multiple providers directly from your workspace
- **Integration Leads** — monitor the performance of your automated data pipeline and manage OAuth connections efficiently to maintain high-reliability standards


## Available Tools
- **list_integrations**: List integration logic configurations available in Nango
- **get_integration**: Retrieve explicit parameters mapping a single target Nango integration
- **list_connections**: List instantiated OAuth or credential connections authenticated via Nango
- **get_connection**: Get exact metadata extracting details mapped to a specific Nango connection
- **list_syncs**: List history or current synchronization status mapped to a connection
- **list_records**: List actual data records synchronized matching a connected provider mapping
- **get_environment**: Retrieve literal environment runtime mapping logic bounds representing the active Nango instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nango (Unified API & Integration Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Salesforce connections in Nango"

**🤖 AI Agent:**
> I've retrieved 12 Salesforce connections. 10 are 'Verified', while 2 (ID: conn-abc, conn-xyz) are currently 'Expired' or 'Invalid'. Would you like me to check the sync status for the verified connections?

---

**👤 You:**
> "Show me the last 5 sync logs for connection ID 'conn-123'"

**🤖 AI Agent:**
> Retrieving sync history… I've identified the 5 most recent syncs for 'conn-123': 4 succeeded (Syncing 'deals'), and 1 'Failed' 2 hours ago with a 'Rate Limit' error. I can provide the detailed error metadata if you'd like.

---

**👤 You:**
> "Fetch the synchronized 'contacts' records for connection 'conn-456'"

**🤖 AI Agent:**
> Executing record extraction… I've retrieved 50 contact records from Nango's unified storage for connection 'conn-456'. Highlights include 'Alex Smith' (id: 987) and 'Sarah Johnson' (id: 654). Would you like to see the full JSON mapping for these records?


## Installation & Usage

To install and use the **Nango (Unified API & Integration Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nango-unified-api-integration-platform](https://vinkius.com/mcp/nango-unified-api-integration-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
