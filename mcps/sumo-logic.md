# Sumo Logic MCP Server

Connect your AI to Sumo Logic. Orchestrate log searches, monitor active collectors, and analyze system events efficiently.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sumo-logic)

## Overview
**Category:** industry-titans
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Sumo Logic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sumo-logic](https://vinkius.com/mcp/sumo-logic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
