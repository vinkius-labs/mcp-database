# Pipedream MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedream)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pipedream-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pipedream-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage Pipedream serverless workflows, sources, webhooks, and raw event data natively via AI agents.

## Description
Connect your **Pipedream** automation workspace directly to any AI agent. Review the architecture of your serverless logic, audit event sources, and inspect real-time transaction limits or logic chains instantly without relying on the browser console.

### What you can do

- **Workflows & Logic** — List and drill down into serverless workflows, viewing configuration limits, step chains, and historical deployment statuses.
- **Event Sources** — Retrieve detailed metadata for any configured Event Source, triggering webhooks, and polling configurations.
- **Real-Time Events** — Intercept and summarize recent, raw physical payload transactions directly ingested by Pipedream endpoints.
- **Webhooks & Subscriptions** — Map active system subscriptions connecting external APIs.

### How it works

1. Subscribe to this Pipedream server integration
2. Provide your Pipedream API Key
3. Start managing your automation logic directly from Claude, Cursor, or your preferred MCP client

### Who is this for?

- **Integration Engineers** — debug webhooks instantly, monitor workflow boundaries, and extract failing source logs directly into coding environments.
- **DevOps Teams** — monitor webhook throughput or event ingest failures dynamically.
- **Automation Builders** — map out complex step trees naturally via the agent without losing context of your broader systems.


## Available Tools
- **list_sources**: List event sources
- **get_source**: Get source details
- **list_workflows**: List workflows
- **get_workflow**: Get workflow details
- **list_events**: List recent events from a source
- **list_subscriptions**: List webhook subscriptions
- **get_user**: Get current user info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipedream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the active event sources parsing my Slack webhooks."

**🤖 AI Agent:**
> You have 3 active HTTP Event Sources currently handling payloads. Source ID `src_xyz` (Slack Notifier) is polling normally, while `src_abc` (Stripe Charges) is temporarily paused due to rate limiting. Need to evaluate the recent transactions from Stripe?

---

**👤 You:**
> "Pull the raw events sent to the source `src_xyz982`."

**🤖 AI Agent:**
> I've pulled the 5 most recent events ingested by `src_xyz982`. The latest transaction executed 3 minutes ago captured a POST request with headers `{ 'content-type': 'application/json' }` and payload `{"user": "jane_doe", "action": "signup"}`. Wait, there's no email object attached. Should we review the workflow logic assigned to handle this?

---

**👤 You:**
> "Describe the node logic in workflow `wf_AByDk`."

**🤖 AI Agent:**
> Workflow `wf_AByDk` consists of 4 distinct steps: 1. `trigger_http` (Webhook inbound). 2. `format_data` (Custom code parsing Node.js strings). 3. `mysql_query` (Writes parameters to database). 4. `send_slack` (Dispatches confirmation notification). Everything appears fully active with zero deployment errors recorded. Would you like the explicit code logic in the `format_data` block?


## Installation & Usage

To install and use the **Pipedream** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedream](https://vinkius.com/mcp/pipedream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
