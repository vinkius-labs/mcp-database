# Temporal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/temporal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Monitor and manage distributed workflows in Temporal Cloud natively via your AI agent.

## Description
Connect your **Temporal Cloud** (or self-hosted) cluster to any AI agent and bring the power of durable execution directly into your IDE or chat via natural conversation.

### What you can do

- **Workflows & Executions** — List, filter, and inspect active, running, or completed workflow executions
- **Workflow History** — Retrieve the complete sequence of events, activities, and signals to debug failures
- **Visibility Search** — Run complex SQL-like queries using Temporal Visibility syntax to find specific runs
- **Namespace Details** — Check retention periods, configurations, and metadata of your operational namespace
- **Schedules & Cron** — Browse all recurring workflows and predict the next execution schedules

### How it works

1. Subscribe to this server
2. Enter your Temporal Address, Namespace, and API Key (or cert pathway)
3. Start querying cluster states strictly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — debug failed workflow runs and retrieve precise event histories without opening the Temporal UI
- **Platform Teams** — audit namespaces and search attributes to ensure data consistency globally
- **Site Reliability Engineers (SREs)** — query complex visibility logs during incident responses


## Available Tools (7)
- **get_workflow_history**: Retrieves the event history for a workflow execution
- **get_namespace_details**: Retrieves information about the current namespace
- **get_workflow_details**: Retrieves details for a specific workflow execution
- **list_schedules**: Lists all workflow schedules
- **list_search_attributes**: Lists custom search attributes available in the namespace
- **list_workflows**: Returns workflow IDs, run IDs, and statuses.

Lists all workflow executions in the configured namespace
- **search_workflows**: g., WorkflowType="MyType" AND Status="Running").

Search workflows using Temporal Visibility Query syntax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temporal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 workflows that failed or panicked in the default namespace."

**🤖 AI Agent:**
> I executed a visibility query for `ExecutionStatus="Failed"`. I found 3 failure records:
- 1. `WithdrawalWorkflow` (Run ID: fca1-4040). Failed at activity `ChargeCreditCard`.
- 2. `SendEmailWorkflow` (Run ID: acb2-2020). Panicked on line 78.
- 3. `OnboardUser` (Run ID: 19ba-3333). Timed out out. Would you like me to pull the full history sequence for any of these to debug?

---

**👤 You:**
> "Explain the exact execution history for workflow 'GenerateInvoice-102'."

**🤖 AI Agent:**
> Here is the summary of events for `GenerateInvoice-102` (Run ID: axd...).
[00:00:01] Workflow execution started.
[00:00:03] Activity `FetchTaxData` scheduled and completed successfully.
[00:00:08] Timer activated for 3 hours.
[03:00:08] Timer fired.
[03:00:10] Activity `SendPDF` failed with a 500 downstream error. Do you want to review the source code behind `SendPDF`?

---

**👤 You:**
> "List all active schedules and tell me when the database backup is due."

**🤖 AI Agent:**
> You have 2 schedules running:
1. `WeeklyReportQueue` (Runs every Monday at 9AM).
2. `DatabaseColdBackup` (Runs daily at Midnight UTC).
According to Temporal, the next execution for `DatabaseColdBackup` is scheduled to start in 5 hours and 14 minutes.


## ❓ FAQ

**Q: Can my AI agent debug a failed Temporal workflow run directly?**
Yes. Instead of browsing the Temporal UI to manually dissect the execution, feed the workflow ID directly to your AI agent. It can seamlessly fetch the entire event history, identify the exact panic line or activity timeout, and immediately suggest code fixes within your IDE.

**Q: How complex can the visibility searches be via natural language?**
Very complex. Because your agent understands your codebase, you can ask 'Find all workflows of type ProcessPayment that failed in the last 2 hours'. The agent formulates the perfect SQL-like syntax for the backend, parses the matching pages, and surfaces exactly which transactions failed.

**Q: Can it read scheduled jobs and Cron jobs configurations inside Temporal?**
Absolutely. You can request a list of all active schedules mapped to your namespace. Your agent unpacks JSON configurations, showing definitions of workflow recurrence, enabling you to detect missing crons without interrupting your workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temporal](https://vinkius.com/mcp/temporal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Temporal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `temporal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Temporal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "temporal": {
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
