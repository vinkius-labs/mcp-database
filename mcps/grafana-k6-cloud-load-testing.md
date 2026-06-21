# Grafana k6 Cloud (Load Testing) MCP Server

Manage load tests via k6 Cloud — run tests, monitor performance metrics, and audit thresholds.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/grafana-k6-cloud-load-testing)

## Overview
**Category:** ship-it
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Grafana k6 Cloud (Load Testing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grafana-k6-cloud-load-testing](https://vinkius.com/mcp/grafana-k6-cloud-load-testing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
