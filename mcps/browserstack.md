# BrowserStack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browserstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browserstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate testing via BrowserStack — manage projects, track test builds, fetch session logs, and monitor execution pipelines from any AI agent.

## Description
Connect your **BrowserStack** Automate account to any AI agent and take full control of your automated cross-browser testing pipeline through natural conversation.

### What you can do

- **Project Management** — List all test projects and drill down into specific project details
- **Build Tracking** — Surface your recent automation builds, their statuses (running, failed, passed), and duration
- **Session Deep Dive** — Retrieve the granular executions of a specific test session, including OS and browser stats
- **Log Extraction** — Automatically dump and analyze the raw Selenium/Appium logs of a failed session
- **Quota & Plan** — View your current plan's parallel session usage and testing queue length
- **Environment Specs** — List all supported OS/browser combinations required to configure your capabilities

### How it works

1. Subscribe to this server
2. Enter your BrowserStack Username and Access Key
3. Start investigating your test suite directly from Claude, Cursor, or any MCP-compatible client

No more context switching to the BrowserStack dashboard just to figure out why a test timed out.

### Who is this for?

- **QA Engineers** — fetch the exact log output of a failing session directly into your IDE for rapid debugging
- **DevOps** — check parallel session concurrency limits and clean up stuck execution sessions
- **Software Developers** — parse build results in natural language without opening the CI/CD test reports
- **Test Automators** — retrieve exact OS/browser configuration payload limits when updating test scripts


## Available Tools
- **list_projects**: json`. Returns project names, IDs, and build counts. Used to organize automation runs.

List all projects on BrowserStack Automate
- **get_project**: json`. This includes name, group ID, and recent builds associated with the project.

Get full details of a BrowserStack project including linked builds
- **list_builds**: json`. Returns build names, IDs, statuses (running/done/timeout/failed), durations, and session counts. Useful for tracking test suite execution.

List recent builds on BrowserStack Automate
- **get_build**: json`. Returns session details, OS/browser combos, results, and logs.

Get all sessions within a BrowserStack automation build
- **get_session**: json`. Includes name, OS, browser, status, reason, duration, video URL, and log URLs.

Get full details of a specific BrowserStack session
- **get_session_logs**: Useful for debugging failed test steps.

Get text execution logs of a BrowserStack session
- **list_browsers**: json`. Returns OS names/versions, browser names/versions required for configuring automation desired capabilities.

List all supported OS/browser combinations on BrowserStack
- **get_plan**: json`, including parallel sessions allowed, team parallel sessions used, queued sessions, and plan name. Essential for managing execution concurrency.

Get current BrowserStack plan details and parallel session usage
- **delete_session**: json`.

Delete a BrowserStack session by ID
- **delete_build**: json`.

Delete a BrowserStack build by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrowserStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent automation builds and summarize their outcomes."

**🤖 AI Agent:**
> You have 4 recent builds:
1. 'Nightly Regression #120' - Passed (Dur: 14:02)
2. 'PR-Check #491' - Passed (Dur: 2:15)
3. 'Payment Flow E2E' - Failed (Dur: 4:30) (Build ID: e4da3b...)
4. 'Hotfix-Deploy-Prod' - Running (Dur: 1:12)

Would you like me to dive into the 'Payment Flow E2E' build and fetch the failed session logs?

---

**👤 You:**
> "Fetch the logs for the failed session in build e4da3b."

**🤖 AI Agent:**
> I retrieved the session inside the build (Session ID: 7a912f). Here is the relevant snippet from the execution logs:

```text
[14:23:45] POST /session/7a912f/element - Request payload: {"using":"css selector","value":"#checkout-btn"}
[14:23:50] NoSuchElementError: no such element: Unable to locate element: {"method":"css selector","selector":"#checkout-btn"}
```

The test failed because the `#checkout-btn` element could not be found after 5 seconds of rendering.

---

**👤 You:**
> "Check how many parallel sessions our current plan allows."

**🤖 AI Agent:**
> According to your `Automate Enterprise` plan, your team is allowed 20 parallel sessions globally. Currently, 18 parallel sessions are in use, and 0 sessions are queued. You have room to start 2 more concurrent threads without throttling.


## Installation & Usage

To install and use the **BrowserStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserstack](https://vinkius.com/mcp/browserstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
