# test-regression-runner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/test-regression-runner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automated verification system that executes targeted test suites and detects regressions or flakiness.

## Description
This MCP server provides tools to automate the verification of code changes. It identifies only the tests affected by specific file modifications, minimizing execution time. By comparing current results against a historical baseline, it detects new failures, removed tests, and non-deterministic flakiness. Use `run_targeted_tests` to execute specific suites, `get_test_baseline` to retrieve previous successful states, and `analyze_regression_differences` to perform deep comparisons between runs.


## Available Tools (3)
- **analyze_regression_differences**: Performs a deep comparison between the current test run results and the baseline
- **run_targeted_tests**: Executes the specific subset of tests identified as being affected by the provided file changes
- **get_test_baseline**: Retrieves the recorded results of the last successful or most recent relevant test run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **test-regression-runner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the tests affected by the changes in src/logic.ts."

**🤖 AI Agent:**
> Tests for src/logic.ts have been executed. Status: PASS. 12 tests passed, 0 failed.

---

**👤 You:**
> "Compare my current test results with the baseline for suite 'core-api'."

**🤖 AI Agent:**
> Comparison complete. 1 new failure detected in 'auth_test.spec.ts'.

---

**👤 You:**
> "Get the baseline for the 'ui-components' suite."

**🤖 AI Agent:**
> Baseline retrieved: lastPassCount: 45, lastFailCount: 0, lastCoverage: 88.5%.


## ❓ FAQ

**Q: How does targeted testing work?**
The system maps modified source files to their corresponding test files using naming conventions, ensuring only relevant tests are run via `run_targeted_tests`.

**Q: What is a regression in this context?**
A regression is a failure in a part of the system that was previously working, identified by comparing the current run against a baseline.

**Q: How can I detect flaky tests?**
You can use `analyze_regression_differences` to identify patterns where tests pass and fail inconsistently without code changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/test-regression-runner](https://vinkius.com/ai-agent-connect/test-regression-runner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **test-regression-runner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `test-regression-runner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **test-regression-runner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "test-regression-runner": {
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
