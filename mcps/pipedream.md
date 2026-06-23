# Pipedream MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedream)
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


## Available Tools (7)
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


## ❓ FAQ

**Q: Can the agent pull raw JSON payloads from specific Pipedream webhooks?**
Yes. Ask the agent to list recent events from a specific Event Source ID. It captures the physical payloads ingested, showing you the raw keys and headers automatically. This is perfect for debugging failed external API calls without leaving your environment.

**Q: How can I trace the steps of my serverless workflow components?**
Request details on a given Workflow ID (`get_workflow`). Your agent will unpack the configuration boundaries, distinct step triggers, and deployment paths, letting you quickly verify logic flow arrays or parameter mappings without needing the web canvas editor.

**Q: Can I have multiple Pipedream workspaces configured?**
Yes, by generating separate API keys per workspace in Pipedream and authenticating them in Vinkius against distinct agents. Use `get_user` to instantly verify which token and quota limit (profile allowances) you are currently mapped onto.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedream](https://vinkius.com/mcp/pipedream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipedream** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipedream` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipedream** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipedream": {
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
