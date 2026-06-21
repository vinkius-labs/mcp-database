# Temporal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/temporal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/temporal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/temporal-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Temporal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/temporal](https://vinkius.com/mcp/temporal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
