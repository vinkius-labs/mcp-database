# Coalesce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coalesce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coalesce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coalesce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enable your AI agent to manage Snowflake data pipelines, trigger transformations, and monitor jobs via the Coalesce API.

## Description
Connect your AI to **Coalesce**, the data transformation platform built for Snowflake with a column-aware approach.

### What you can do

- **Environment Management** — List all environments in your Coalesce organization and inspect their configurations.
- **Job Monitoring** — Check the status of the last run for any environment and view execution logs.
- **Trigger Transformations** — Start transformation jobs on demand with optional node selectors to target specific pipelines.

### How it works

1. Add the Coalesce integration to your AI toolset.
2. Provide your API Token (from Organization Settings > API Tokens).
3. Manage your data pipelines via natural language.

### Who is this for?

- **Data Engineers** — Trigger and monitor pipeline runs without opening the Coalesce UI.
- **Analytics Engineers** — Check job statuses and debug failed transformations from chat.
- **Data Team Leads** — Get quick overviews of environment health and recent job results.


## Available Tools
- **get_environment**: Retrieve detailed information about a specific environment
- **get_job_details**: Retrieve detailed information about a specific job
- **get_run_status**: Check the current status and progress of a triggered run
- **list_environments**: Retrieve all environments configured in your Coalesce organization
- **list_jobs**: Retrieve a list of jobs, optionally filtered by environment
- **list_nodes**: Retrieve metadata about transformation nodes in a specific environment
- **trigger_job**: Trigger a specific job in an environment
- **trigger_run**: Trigger a new run for a specific environment and optionally a job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coalesce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all environments in my Coalesce organization."

**🤖 AI Agent:**
> You have 3 environments:
1. 'Production' (env-001) — Last run: success, 2h ago
2. 'Staging' (env-002) — Last run: success, 5h ago
3. 'Development' (env-003) — Last run: failed, 1h ago
Would you like to check the failed run details?

---

**👤 You:**
> "Trigger job 'job-yyyy' in environment 'env-xxxx'."

**🤖 AI Agent:**
> Job 'job-yyyy' triggered in environment 'env-xxxx'. Run ID: run-8k3m. Status: running. Estimated completion: ~4 minutes.

---

**👤 You:**
> "What is the status of the ongoing production data pipeline?"

**🤖 AI Agent:**
> The production pipeline (Run ID: run-9g1l) is currently at 85%. All dimension tables have refreshed successfully, and the fact nodes are currently materializing in Snowflake.


## Installation & Usage

To install and use the **Coalesce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coalesce](https://vinkius.com/mcp/coalesce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
