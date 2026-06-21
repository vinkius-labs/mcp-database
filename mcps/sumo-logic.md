# Sumo Logic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sumo-logic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect your AI to Sumo Logic. Orchestrate log searches, monitor active collectors, and analyze system events efficiently.

## Description
Empower your AI workflows with the powerful machine data analytics computing of **Sumo Logic**. Connect your conversational interface to your security, incident management, and monitoring environments, enabling your LLM to actively query diagnostic logs, monitor data ingestion pipelines securely, and track account consumption seamlessly. Automate log analysis organically from the terminal, avoiding complex dashboard integrations entirely.

### What you can do

- **Log Search & Diagnosis** — Formulate deep queries into your data leveraging `create_search_job`, track asynchronous execution with `get_search_status`, and securely fetch the resultant incident analytics running `get_search_results`.
- **Data Ingestion Monitoring** — Systematically browse telemetry sources assigning context mapping via `list_collectors` and inspect granular configurations evaluating `get_collector_details`.
- **Account Administration** — Enforce operational compliance rapidly evaluating access levels using `list_account_roles` and inspecting associated internal teams via `list_account_users`.
- **Operations Analytics** — Trace organizational usage data assessing `get_account_billing` and confirm external alert hookings directly mapping systems via `list_active_webhooks`.

### How it works

1. Enable the Sumo Logic MCP integration module in your Vinkius environment.
2. In the parameter settings, authenticate securely using your standard `SUMO_ACCESS_ID` alongside your `SUMO_ACCESS_KEY` directly from your administrative dashboard.
3. Instruct your artificial intelligence naturally: "Run a log search on our production cluster for 'timeout errors' spanning the last 2 hours, wait for completion, and summarize the recurring IPs."

### Who is this for?

- **DevOps Engineers** — Debug and resolve incidents rapidly without switching screens, utilizing precise searches right at the conversational terminal mapping root causes.
- **Site Reliability Engineers (SREs)** — Validate data ingest loads, track platform limits dynamically, and evaluate webhook configurations accurately and efficiently.
- **Security Operations Analyists (SecOps)** — Evaluate log trails and access control parameters concurrently directly securely exploring logs independently from web consoles.


## Available Tools
- **list_account_users**: Lists all registered users in the account
- **list_active_webhooks**: Lists configured alert webhooks
- **create_search_job**: Provide a query string, start time, and end time. Returns a search job ID for tracking.

Creates a new log search job
- **get_account_billing**: Retrieves billing and usage metrics
- **get_collector_details**: Retrieves details for a specific collector
- **get_search_results**: Retrieves the results of a completed search job
- **get_search_status**: Retrieves the status of an existing search job
- **list_collectors**: Lists all data collectors configured in Sumo Logic
- **list_account_roles**: Lists all security roles in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sumo Logic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch all account users along with active local integration webhooks sequentially properly."

**🤖 AI Agent:**
> Authenticating logic cleanly verifying parameters safely accurately...
**Account Operatives Located (`list_account_users`)**:
- `Sarah Connor (s.connor@sumo.io)` - Admin
- `John Ops (j.ops@sumo.io)` - Observer

**External Endpoints Mapped Systematically (`list_active_webhooks`)**:
- `PagerDuty Alerts` (Status: Active)
- `Slack #sec-ops channel` (Status: Active)
Successfully executed read tasks seamlessly inherently securely clearly effectively.

---

**👤 You:**
> "Create a new search job tracking 'auth_failure' errors over the last 24 hours."

**🤖 AI Agent:**
> Initiating search constraints flawlessly...
Executed `create_search_job` cleanly, allocating Job ID `881A-9XF` securely.
Actively parsing `get_search_status` locally:
- Check 1: Processing dynamically.
- Check 2: Resolution Finalized accurately.
Status natively secured actively.

---

**👤 You:**
> "Retrieve the exact search results from the active job ID once the asynchronous monitoring reports completion."

**🤖 AI Agent:**
> Retrieving output systematically and faithfully...
**Log Occurrences Captured via `get_search_results` natively**:
- Incident 08:00 AM: IP 10.4.5.1 failed authentication structurally.
- Incident 11:30 AM: IP 192.168.1.10 unauthorized access attempt.
Search results retrieved seamlessly.


## ❓ FAQ

**Q: How does the AI handle asynchronous search jobs properly since large logs take time natively?**
The integration specifically manages this asynchronously. The AI invokes `create_search_job` effectively obtaining a unique job tracking ID. It autonomously utilizes `get_search_status` routinely actively safely until the task reports resolution, seamlessly proceeding afterwards intelligently triggering `get_search_results` natively securely.

**Q: Can this integration edit user parameters, manage collectors fundamentally, or delete billing records?**
No, this module functions predominantly securely executing read-only investigations or orchestrating transient analytical read capabilities (creates logically secure temporal jobs). Destructive modifications fundamentally affecting users, collectors realistically securely actively explicitly structurally are avoided completely securely internally naturally globally by architectural design.

**Q: Which log sources can the AI query through this integration?**
Any source ingested by your Sumo Logic collectors — application logs, infrastructure metrics, cloud audit trails, and custom HTTP sources. The AI queries them all through the unified search API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sumo-logic](https://vinkius.com/mcp/sumo-logic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sumo Logic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sumo-logic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sumo Logic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sumo-logic": {
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
