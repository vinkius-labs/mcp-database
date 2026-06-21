# Katalon TestOps (AI Test Management) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/katalon-testops-ai-test-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/katalon-testops-ai-test-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/katalon-testops-ai-test-management-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage test orchestration via Katalon TestOps — rerun test runs, monitor execution results, and audit software releases.

## Description
Connect your **Katalon TestOps** account to any AI agent and take full control of your AI-powered test management and quality orchestration through natural conversation.

### What you can do

- **Execution Orchestration** — List all test runs and trigger immediate re-executions of specific suites to verify bug fixes directly from your agent
- **Quality Analytics** — Retrieve detailed test outcome summaries, including pass/fail rates, execution durations, and error stack traces
- **Diagnostic Inspection** — Deep-dive into individual test results to extract application logs, error messages, and visual screenshots for rapid debugging
- **Environment Audit** — List configured execution environments to understand target OS, browser, and device distributions across your projects
- **Release Management** — Monitor defined software releases and track aggregated test run statistics to ensure build quality before deployment
- **Project CRM** — Navigate across multiple Katalon projects and retrieve detailed metadata including team assignments and suite counts securely

### How it works

1. Subscribe to this server
2. Enter your Katalon Email and API Key
3. Start managing your test orchestration from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — monitor release readiness and track team testing progress through natural conversation without jumping between projects
- **Automation Engineers** — rerun failed test suites and inspect diagnostic logs directly from your workspace for rapid iteration
- **DevOps Engineers** — audit execution environments and verify build quality results to ensure CI/CD pipeline integrity


## Available Tools
- **list_projects**: Returns project names, IDs, and descriptions.

List all projects on Katalon TestOps
- **get_project**: Get full details of a Katalon project
- **list_test_runs**: Returns run IDs, pass/fail status, total counts, and execution durations.

List test runs within a Katalon project
- **get_test_run**: Get full details of a Katalon test run
- **rerun_test_run**: Returns the newly created test run ID.

Re-run an existing Katalon test run
- **list_test_results**: Returns durations, statuses, and error messages.

List detailed test results within a test run
- **get_test_result**: Get full details of a single Katalon test result
- **list_execution_environments**: List execution environments in a Katalon project
- **list_project_releases**: Returns release names, scheduled dates, and aggregated test run statistics.

List defined releases in a Katalon project
- **list_project_builds**: Returns build identifier names, IDs, and the count of associated test runs.

List software builds in a Katalon project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Katalon TestOps (AI Test Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 test runs in project 'E-commerce API' (ID: 123)"

**🤖 AI Agent:**
> I've retrieved the latest 5 test runs for project 123. Highlights: Run #987 (Passed), Run #986 (Failed - 2 errors), Run #985 (Passed). Would you like to inspect the results for the failed run?

---

**👤 You:**
> "Rerun test run ID 986"

**🤖 AI Agent:**
> Rerunning test run 986… New active execution started. New Run ID: 988. I'll let you know once the results are available. Would you like me to notify you if it fails again?

---

**👤 You:**
> "What are the active releases defined in project 123?"

**🤖 AI Agent:**
> I've identified 2 active releases in project 123: 'Q1 Spring Update' (v1.2.0) and 'Hotfix Security' (v1.2.1). Release v1.2.0 has 45 associated test runs with a 98% pass rate. Would you like a detailed build report?


## Installation & Usage

To install and use the **Katalon TestOps (AI Test Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/katalon-testops-ai-test-management](https://vinkius.com/mcp/katalon-testops-ai-test-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
