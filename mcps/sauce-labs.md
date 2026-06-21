# Sauce Labs MCP Server

Monitor and manage UI/E2E test automation at scale via AI — stop failing jobs, inspect video logs, and check pipeline concurrency metrics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sauce-labs)

## Overview
**Category:** ship-it
**Tools Count:** 11

## Description
Connect your **Sauce Labs** account to any AI agent to bring your entire test execution landscape directly into your chat workflow. Say goodbye to jumping between CI/CD tools and the Sauce Labs dashboard to investigate failures.

### What you can do

- **Jobs & Builds** — Check the status of recent test builds, drill down into specific job results, and monitor pass/fail ratios
- **Incident Management** — Programmatically stop hung or failing jobs to free up test concurrency limits instantly
- **Infrastructure Metrics** — Check your active Sauce Connect tunnels, current account activity, and real-time concurrency metrics
- **Platform Support** — Browse supported OS and browser combinations (Appium, WebDriver) directly through the agent

### How it works

1. Subscribe to this server
2. Provide your Sauce Labs Username, Access Key, and operating Region
3. Start monitoring your automation suite from Claude, Cursor, or any MCP-compatible client

Your AI agent will be able to pinpoint specific build failures, analyze error trace metadata, and keep your software delivery pipeline healthy.

### Who is this for?

- **QA Engineers** — quickly look up the video or log output of a specific failed Selenium/Playwright job without finding it in the dashboard
- **DevOps** — check active Sauce Connect tunnels and current concurrency limits when tests start queuing unexpectedly
- **Developers** — verify available browser/OS configurations on the fly when adding a new matrix variable to a test suite


## Available Tools
- **get_activity**: Retrieves current account activity levels
- **get_build_jobs**: Lists all individual jobs within a specific build
- **get_build**: Retrieves details for a specific build
- **get_concurrency**: Retrieves account concurrency limits
- **get_job**: Retrieves details for a specific test job
- **get_status**: Checks current Sauce Labs platform availability
- **list_builds**: Lists recent automation builds
- **list_jobs**: ).

Lists recent test jobs on Sauce Labs
- **list_platforms**: Specify all, appium, or webdriver.

Lists all supported OS and browser combinations
- **list_tunnels**: Lists active Sauce Connect tunnels
- **stop_job**: Stops a running test job


## Installation & Usage

To install and use the **Sauce Labs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sauce-labs](https://vinkius.com/mcp/sauce-labs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
