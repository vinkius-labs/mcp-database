# Grafana k6 Cloud (Load Testing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana-k6-cloud-load-testing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage load tests via k6 Cloud — run tests, monitor performance metrics, and audit thresholds.

## Description
Connect your **Grafana Cloud k6** account to any AI agent and take full control of your performance engineering and load testing lifecycle through natural conversation.

### What you can do

- **Test Orchestration** — List all cloud-hosted load tests and retrieve detailed script configurations and Virtual User (VU) setups directly from your agent
- **Execution Management** — Start new test runs on k6 Cloud infrastructure and abort active executions instantly to manage system resources
- **Metrics Analytics** — Retrieve aggregated performance metrics (latency, error rates, throughput) for completed runs to understand system behavior under load
- **Threshold Audit** — Get detailed threshold evaluation results to verify if your application meets specific SLOs and performance requirements
- **Organization & Projects** — Navigate across multiple organizations and projects to manage complex testing environments securely
- **Real-time Monitoring** — Poll ongoing test runs to track status transitions (QUEUED, RUNNING, FINISHED) and total execution durations

### How it works

1. Subscribe to this server
2. Enter your k6 Cloud API Token
3. Start managing your load tests from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance Engineers** — trigger load tests and analyze metrics through natural conversation without jumping between dashboards
- **DevOps & SREs** — monitor application thresholds and verify performance regressions after recent deployments
- **QA Automation** — audit test run histories and report on overall system reliability across different environments efficiently


## Available Tools
- **list_tests**: Returns test names, IDs, scripts, and last run statuses.

List all load tests on Grafana Cloud k6
- **get_test**: Get full details of a k6 test
- **list_runs**: Returns run IDs, status states (QUEUED/RUNNING/FINISHED/ABORTED), VU counts, durations, and timestamps.

List test runs for a specific k6 test
- **get_run**: Get full details of a k6 test run
- **start_test_run**: Returns the new active run ID for tracking.

Start a new k6 Cloud test run
- **stop_test_run**: Stop a running k6 Cloud test
- **list_organizations**: Returns organization names, IDs, and member counts.

List organizations on k6 Cloud
- **list_projects**: Projects contain tests.

List projects in a k6 Cloud organization
- **get_run_metrics**: g., http_req_duration, http_req_failed, iterations, VUs, data_received, etc.).

Get performance metrics for a k6 run
- **get_run_thresholds**: Get threshold evaluation results for a k6 run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grafana k6 Cloud (Load Testing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my load tests in k6 Cloud"

**🤖 AI Agent:**
> I've found 4 load tests: 'API Stress Test' (ID: 123), 'Checkout Flow' (ID: 456), 'Inventory Spike' (ID: 789), and 'Frontend Smoke' (ID: 012). Which one would you like to check the last run status for?

---

**👤 You:**
> "Show me the performance metrics for the last run of the 'API Stress Test'"

**🤖 AI Agent:**
> Retrieving metrics for run ID 'run-98765'… Average response time: 142ms, P95: 285ms, Failed requests: 0.2%, Max VUs: 500. All metrics are within acceptable ranges. Would you like me to check the threshold details?

---

**👤 You:**
> "Start a new test run for 'Checkout Flow' (ID: 456)"

**🤖 AI Agent:**
> Trigging new run for 'Checkout Flow'… Done. New Run ID is 'run-13579'. It's currently in the QUEUED state. I'll let you know when the first VUs start injecting traffic.


## ❓ FAQ

**Q: Can I see if a load test passed its performance thresholds using my agent?**
Yes. Use the `get_run_thresholds` tool with a specific Run ID. Your agent will retrieve the final evaluation for all defined thresholds in the script, indicating which specific SLOs passed or failed.

**Q: How do I start a new k6 Cloud test run through a conversation?**
Use the `start_test_run` tool by providing the Test ID. Your agent will trigger the execution on k6 Cloud infrastructure and return an active Run ID that you can use to track real-time progress.

**Q: Can my agent retrieve the raw performance metrics for a completed run?**
Absolutely. The `get_run_metrics` tool allows your agent to aggregate data like `http_req_duration`, error counts, and total iterations, providing a rapid summary of your application's behavior under load.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana-k6-cloud-load-testing](https://vinkius.com/mcp/grafana-k6-cloud-load-testing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grafana k6 Cloud (Load Testing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grafana-k6-cloud-load-testing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grafana k6 Cloud (Load Testing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grafana-k6-cloud-load-testing": {
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
