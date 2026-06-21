# LambdaTest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lambdatest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test your website and apps across thousands of real browsers and devices in the cloud with automated and manual testing tools.

## Description
Connect your **LambdaTest** account to any AI agent and manage browser testing through natural conversation.

### What you can do

- **Build Management** — List builds, inspect results, and track pass/fail rates
- **Session Tracking** — Browse test sessions with logs, screenshots, and video recordings
- **Test Results** — Monitor test outcomes across browsers and platforms
- **Automation Logs** — Access detailed execution logs for debugging
- **Platform Info** — Browse available browser/OS combinations for testing

### How it works

1. Subscribe to this server
2. Enter your LambdaTest Username and Access Key
3. Start managing tests from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — track test builds and analyze failures
- **Developers** — review automation logs and session recordings
- **Test Leads** — monitor cross-browser test coverage and results


## Available Tools (7)
- **get_build_details**: Get metadata for a build
- **get_test_logs**: Retrieve execution logs
- **get_session_details**: Get metadata for a test run
- **list_automation_builds**: Supports filtering by status.

List your LambdaTest builds
- **list_supported_platforms**: List OS/Browser combinations
- **list_test_sessions**: Supports filtering by build_id.

List individual test runs
- **update_session_status**: Set the outcome of a test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LambdaTest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all builds and the latest test results."

**🤖 AI Agent:**
> Builds: 12 total. Latest: Build #45 — 'Regression Suite' (42 tests, 38 passed ✅, 3 failed ❌, 1 error ⚠️). Build #44 — 'Smoke Tests' (15 tests, 15 passed ✅). Build #43 — 'Cross-browser' (28 tests, 26 passed, 2 failed). Pass rate (7 days): 91%. Failed tests in Build #45: 'Login Page — Firefox 120', 'Checkout — Safari 17', 'Search — Edge 121'.

---

**👤 You:**
> "Show the session details and screenshots for the failed login test."

**🤖 AI Agent:**
> Session: 'Login Page — Firefox 120'. Status: ❌ Failed. Duration: 45s. Browser: Firefox 120.0 / Windows 11. Error: Element not found '#submit-btn' (timeout after 10s). Screenshots: 3 captured. Step 1: Page loaded ✅. Step 2: Email entered ✅. Step 3: Submit click ❌ (element missing). Video recording: available (45s). Console errors: 1 — 'Uncaught TypeError: Cannot read property of null'.

---

**👤 You:**
> "List available browsers and recent automation run statistics."

**🤖 AI Agent:**
> Browsers: Chrome (118-124), Firefox (115-121), Safari (16-17), Edge (118-124), Opera (104-108). OS: Windows 11/10/8, macOS Sonoma/Ventura/Monterey, Ubuntu 22/20. Stats (30 days): 456 sessions, 38 builds, 91.2% pass rate. Average duration: 2.3 min. Most tested: Chrome 124/Win11 (180 sessions). Flaky tests: 4 identified.


## ❓ FAQ

**Q: Can I view test builds and session results?**
Yes. List all builds with pass/fail counts, browse individual sessions with screenshots, video recordings, and detailed execution logs.

**Q: Does LambdaTest use Basic Auth?**
Yes. LambdaTest uses **HTTP Basic Auth** with your Username and Access Key (Base64 encoded) against `api.lambdatest.com/automation/api/v1`.

**Q: Can I browse available browser and OS combinations?**
Yes. Access the full list of supported browsers, versions, and operating systems for cross-browser testing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lambdatest](https://vinkius.com/mcp/lambdatest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LambdaTest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lambdatest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LambdaTest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lambdatest": {
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
