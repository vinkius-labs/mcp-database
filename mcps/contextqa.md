# ContextQA MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contextqa)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contextqa-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contextqa-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate testing via ContextQA — manage test suites, track AI-healing executions, trigger automated runs, and audit API tests directly from any AI agent.

## Description
Connect your **ContextQA** account to any AI agent and take full control of your context-aware AI testing platform through natural conversation.

### What you can do

- **Project & Suite Management** — List bounded test environments and perform structural extraction of GUI test suites across your projects
- **AI-Healing Executions** — Monitor active test runs and inspect specific AI-healing states, including failing step boundaries and screen captures
- **Automated Triggers** — Dispatch live testing commands to queue suites against ContextQA test clusters directly from your workspace
- **API & Swagger Testing** — Enumerate automated HTTP assertions and explicitly verify structural payloads against OpenAPI configurations
- **Environment Auditing** — List physical runtime URLs and group active contexts to verify testing boundaries across different layers
- **Test Case Inspection** — Resolve AI root-cause models and validate specific case definitions to identify precise points of failure

### How it works

1. Subscribe to this server
2. Enter your ContextQA API Key (found in your Dashboard Settings > API Keys)
3. Start managing your automated testing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — trigger test runs and monitor AI-healing execution results without leaving the chat
- **DevOps Teams** — audit test suite coverage and monitor pipeline integration statuses in real-time
- **Software Developers** — verify API test payloads and inspect failed test case boundaries directly from the IDE
- **Product Owners** — monitor release readiness and audit test execution history using natural language


## Available Tools
- **list_projects**: Identify bounded ContextQA test environments grouping automated validations
- **get_project**: Retrieve explicit Project mapping UUIDs analyzing execution spaces limitlessly
- **list_suites**: Perform structural extraction matching asynchronous GUI test Suites payloads
- **list_cases**: Discover explicit routing limits structuring ContextQA cases trees
- **get_case**: Validate Data Science object extraction tracking explicit steps boundaries
- **list_executions**: Inspect deep internal interaction tracking explicit global Run chunks
- **get_execution**: Execute static queries targeting exactly specific AI-healing Run states
- **list_environments**: List static configurations mapping Environment target layers mapping limits
- **list_api_tests**: Extracts native REST & OpenAPI testing configurations natively
- **trigger_run**: Dispatch a live testing command routing explicit Jobs against pipelines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ContextQA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all test suites for project 'vinkius-app-prod'"

**🤖 AI Agent:**
> I found 4 suites in 'vinkius-app-prod': 'Checkout-Flow', 'User-Onboarding', 'API-Security-Scan', and 'Mobile-Sanity'. Which one would you like to audit or trigger?

---

**👤 You:**
> "Trigger a run for suite 'Checkout-Flow' in project 'vinkius-app-prod'"

**🤖 AI Agent:**
> Test run triggered! Suite 'Checkout-Flow' has been queued. You can monitor the progress using Execution ID 'exec_123'. I will notify you once the AI-healing analysis is complete.

---

**👤 You:**
> "Show me why the last execution of project 'mobile-app' failed"

**🤖 AI Agent:**
> Analyzing last execution for 'mobile-app'... It failed at step 5: 'Click Login Button'. The element was not found. ContextQA's AI-healing attempted to locate it but failed due to a structural change in the DOM.


## Installation & Usage

To install and use the **ContextQA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contextqa](https://vinkius.com/mcp/contextqa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
