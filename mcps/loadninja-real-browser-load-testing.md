# LoadNinja (Real-Browser Load Testing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loadninja-real-browser-load-testing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/loadninja-real-browser-load-testing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/loadninja-real-browser-load-testing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage performance tests via LoadNinja — trigger load scenarios, monitor metrics, and audit virtual user (VU) limits.

## Description
Connect your **LoadNinja** account to any AI agent and take full control of your real-browser load testing and performance engineering lifecycle through natural conversation.

### What you can do

- **Scenario Orchestration** — List all LoadNinja scenarios and retrieve detailed configuration trees, including target URLs and step layouts directly from your agent
- **Live Load Injection** — Trigger new test runs with specified virtual users (VUs) and duration to simulate high-traffic real-browser behavior globally
- **Performance Analytics** — Extract aggregated summaries tracking throughput, peak VU mappings, and transaction lengths for completed test runs securely
- **Diagnostic Metrics** — Retrieve raw performance statistics and server response times to identify bottlenecks under heavy application load
- **Operational Control** — Instantly vaporize active running tests to manage system resources or halt erroneous load cycles in real-time
- **Grid Visibility** — Discover available native browser variants and physical data center locations for global load injection auditing

### How it works

1. Subscribe to this server
2. Enter your LoadNinja API Key
3. Start managing your performance infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance Engineers** — trigger complex load scenarios and analyze throughput metrics through natural conversation without manual report exports
- **QA Automation Teams** — monitor test run completion statuses and verify performance regressions directly from your workspace
- **DevOps Engineers** — audit virtual user (VU) limits and data center locations to ensure global scalability and infrastructure reliability


## Available Tools
- **list_scenarios**: List all load test scenarios on LoadNinja
- **get_scenario**: Get full details of a specific LoadNinja scenario including target URL and configuration
- **run_scenario**: Run a LoadNinja scenario with specified virtual users and duration explicitly in minutes
- **list_test_runs**: List all test executions reporting active completion status on LoadNinja
- **get_test_run**: Get full details and summaries of a specific LoadNinja completed test run
- **get_test_run_stats**: Get raw performance statistics for a specific LoadNinja test run
- **stop_test_run**: Irreversibly vaporize an active running LoadNinja test immediately
- **list_browsers**: List available explicit native browsers configured on LoadNinja
- **list_locations**: List available explicit physical data center load injection locations
- **get_account**: Get precise LoadNinja bound subscription account details and strict runtime VU limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LoadNinja (Real-Browser Load Testing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all load test scenarios in my LoadNinja account"

**🤖 AI Agent:**
> I've found 4 scenarios: 'Main-Store-Checkout' (ID: scen-123), 'User-Login-Flow' (ID: scen-456), 'Inventory-Search-API' (ID: scen-789), and 'Mobile-App-Smoke' (ID: scen-012). Which one would you like to run or inspect?

---

**👤 You:**
> "Run scenario 'scen-123' with 100 VUs for 10 minutes"

**🤖 AI Agent:**
> Triggering load test scenario 'scen-123'… I've started the run with 100 virtual users for a duration of 10 minutes. New Run ID: 'run-98765'. I'll monitor the progress and notify you once the performance metrics are available.

---

**👤 You:**
> "Show me the performance stats for the last completed run"

**🤖 AI Agent:**
> Retrieving metrics for run ID 'run-13579'… The test achieved a peak of 250 VUs with an average throughput of 45 requests/sec. The P95 transaction duration was 1.2s. No major bottlenecks detected. Would you like to see the raw metrics breakdown?


## Installation & Usage

To install and use the **LoadNinja (Real-Browser Load Testing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loadninja-real-browser-load-testing](https://vinkius.com/mcp/loadninja-real-browser-load-testing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
