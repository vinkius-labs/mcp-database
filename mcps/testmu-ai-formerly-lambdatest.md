# TestMu AI (formerly LambdaTest) MCP Server

Manage cross-browser testing via TestMu AI — audit automation builds, inspect test sessions, and retrieve visual logs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/testmu-ai-formerly-lambdatest)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Connect your **TestMu AI (formerly LambdaTest)** account to any AI agent and take full control of your cross-browser testing and automation orchestration through natural conversation.

### What you can do

- **Build Orchestration** — List all test automation builds and retrieve high-level aggregated telemetry for Selenium, Playwright, or Cypress suites directly from your agent
- **Session Inspection** — Deep-dive into individual browser test sessions to extract console errors, network configurations, and exact metadata required for rapid debugging
- **Visual Artifacts** — Fetch absolute URLs for bug screenshots and full video recordings of browser executions to reproduce flakey UI issues instantly
- **Precision Logging** — Extract command-level logs including W3C WebDriver protocols or Playwright RPC calls with precise execution timestamps
- **Tunnel & Platform Audit** — Monitor active secure tunnels for localhost testing and query the grid for supported macOS, Windows, iOS, and Android capabilities
- **Environment Mapping** — Filter and retrieve all child test sessions nested under specific CI/CD builds to isolate and analyze deployment regressions

### How it works

1. Subscribe to this server
2. Enter your TestMu AI Username and Access Key
3. Start managing your testing grid from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Automation Engineers** — monitor build health and inspect diagnostic logs through natural conversation without leaving your IDE or switching to the dashboard
- **Software Developers** — retrieve session screenshots and videos to debug UI failures directly from your workspace for rapid iteration
- **DevOps Teams** — audit CI/CD test results and monitor secure tunnel connections across different testing environments efficiently


## Available Tools
- **list_builds**: Groups thousands of executed Selenium, Cypress, Playwright, or Appium browser tests into their respective parent CI/CD builds.

List all test automation builds on LambdaTest Cloud
- **get_build**: Get exact telemetry for a specific LambdaTest build
- **list_sessions**: Provides OS, Browser version, execution duration, and final completion status of the Selenium/Playwright scripts.

List recent automated test sessions executed on LambdaTest
- **get_session**: Identifies explicit console errors, network configuration, and URL artifacts necessary to debug why a specific UI interaction failed.

Get deep context for a specific automated test session
- **get_session_logs**: Extract precise Selenium/Appium command logs for a test
- **get_screenshots**: saveScreenshot()` or failure-hook logic within the LambdaTest grid.

Fetch visual bug screenshots captured during a test session
- **get_video**: Retrieve the full video recording URL for a test execution
- **list_tunnels**: List all active secure Tunnels (UnderTest tunnels)
- **list_platforms**: Returns exactly which combinations of macOS, Windows, iOS, and Android versions are actively available in the testing grid.

List all supported OS/browser capabilities available
- **get_build_sessions**: Extract all explicit test sessions associated with a Build


## Installation & Usage

To install and use the **TestMu AI (formerly LambdaTest)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/testmu-ai-formerly-lambdatest](https://vinkius.com/mcp/testmu-ai-formerly-lambdatest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
