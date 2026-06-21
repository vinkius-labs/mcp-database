# Sauce Labs MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sauce-labs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sauce-labs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sauce-labs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Monitor and manage UI/E2E test automation at scale via AI — stop failing jobs, inspect video logs, and check pipeline concurrency metrics.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sauce Labs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current concurrency usage vs limit in Sauce Labs?"

**🤖 AI Agent:**
> I checked your concurrency data. You are currently using 12 out of your 25 allowed parallel sessions. There are currently no queued jobs. You have plenty of capacity to spin up a new test run.

---

**👤 You:**
> "Show me the jobs that failed in my last automation build."

**🤖 AI Agent:**
> In your most recent build ('Nightly Regression 2.4.1'), exactly 1 out of 45 jobs failed. Job ID: fbd198. The failure occurred on Chrome version 114 (Windows 10). Would you like the deep link to the video asset or the error log for this job?

---

**👤 You:**
> "Stop the test job ID 4f4f391e0 because it's stuck."

**🤖 AI Agent:**
> I've successfully terminated Job ID 4f4f391e0. The status has changed to 'aborted' and the underlying machine node has been freed, releasing 1 concurrent session to the pool.


## Installation & Usage

To install and use the **Sauce Labs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sauce-labs](https://vinkius.com/mcp/sauce-labs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
