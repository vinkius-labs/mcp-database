# BrowserStack MCP Server

Automate testing via BrowserStack — manage projects, track test builds, fetch session logs, and monitor execution pipelines from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/browserstack)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **BrowserStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserstack](https://vinkius.com/mcp/browserstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
