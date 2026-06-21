# Cypress Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cypress-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cypress-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cypress-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Audit E2E testing via Cypress — monitor test runs, inspect spec instances, track flaky tests, and generate enterprise reports directly from any AI agent.

## Description
Connect your **Cypress Cloud** enterprise account to any AI agent and take full control of your end-to-end testing lifecycle and quality metrics through natural conversation.

### What you can do

- **Run Monitoring** — List recent test executions for your projects and retrieve detailed passed/failed/pending counts and commit info
- **Instance Deep Dives** — Inspect specific spec file executions to retrieve error messages, screenshots, and video URLs for failed tests
- **Flaky Test Identification** — Generate enterprise reports to identify intermittent failures and audit last flake dates across your codebase
- **Performance Auditing** — Retrieve slow test reports to evaluate average durations and p95 performance metrics for your CI/CD pipeline
- **Enterprise Reporting** — Fetch aggregated run summaries and granular test result data formatted for BI dashboards and audits
- **Project Navigation** — List all organizational projects and identify unique 6-character IDs required for programmatic data extraction

### How it works

1. Subscribe to this server
2. Enter your Cypress Cloud Enterprise API Key and your Project ID
3. Start auditing your E2E test results from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — monitor test run statuses and identify the root cause of failures using natural language
- **DevOps Teams** — audit pipeline performance and track flaky tests to improve CI reliability
- **Software Developers** — fetch test results and error logs directly from the IDE or development workspace
- **Engineering Managers** — monitor overall project quality and maintainability through automated enterprise reports


## Available Tools
- **list_projects**: Useful for finding the `project_id`.

List all projects on Cypress Cloud. Cypress is the leading JavaScript E2E testing framework. Returns project names, IDs, and org info via the Enterprise Data Extract API
- **get_runs**: List recent test runs for a Cypress Cloud project. Returns run IDs, commit info, branch, CI build IDs, statuses (passed/failed/running), durations, and spec counts
- **get_run**: Get full details of a Cypress Cloud run including status, total tests, passed/failed/pending counts, duration, parallelization, groups, and commit info
- **get_instances**: List spec instances within a Cypress run. Each instance represents one spec file execution. Returns instance IDs, spec names, statuses, and durations
- **get_instance**: Get full details of a Cypress spec instance including spec name, status, error messages, screenshots, video URLs, and browser info
- **get_tests**: List individual tests within a Cypress spec instance. Returns test titles, states (passed/failed/pending/skipped), durations, and error messages
- **report_runs**: Must provide the start date.

Get enterprise run summary report from Cypress Cloud. Aggregated data for BI dashboards. Requires start_date (YYYY-MM-DD)
- **report_tests**: Get enterprise test results report from Cypress Cloud. Individual test-level data with statuses and error messages
- **report_flaky**: Get flaky test report from Cypress Cloud. Identifies tests that intermittently pass/fail. Returns test names, flake rates, and last flake dates
- **report_slow**: Get slow test report from Cypress Cloud. Identifies slowest tests by average duration. Returns test names, avg/p95/max durations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cypress Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 test runs for project 'abc123'"

**🤖 AI Agent:**
> I found 5 recent runs for project 'abc123'. The latest run (ID: 101) finished with status 'Passed' on the 'main' branch. Run 99 failed with 2 failing specs. Would you like to see the details for the failed run?

---

**👤 You:**
> "Show me why instance 'ins_789' failed"

**🤖 AI Agent:**
> Retrieving details for instance 'ins_789'... It failed during 'Login spec'. Error: 'Timed out retrying after 4000ms: Expected to find element: .login-success, but never found it.' I have the video and screenshot links available.

---

**👤 You:**
> "Give me a report of flaky tests starting from 2024-01-01"

**🤖 AI Agent:**
> Analyzing flaky tests since Jan 1st... I identified 3 flaky tests. 'Checkout flow' has a 15% flake rate, and 'User profile update' has flaked twice this month. I can list the last flake dates for these.


## Installation & Usage

To install and use the **Cypress Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cypress-cloud](https://vinkius.com/mcp/cypress-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
