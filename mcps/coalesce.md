# Coalesce MCP Server

Enable your AI agent to manage Snowflake data pipelines, trigger transformations, and monitor jobs via the Coalesce API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coalesce)

## Overview
**Category:** developer-tools
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Coalesce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coalesce](https://vinkius.com/mcp/coalesce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
