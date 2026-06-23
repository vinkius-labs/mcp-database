# Mabl (AI-Powered Test Automation) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mabl-ai-powered-test-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage E2E testing via Mabl — trigger test plans, monitor execution results, and perform AI-driven failure analysis.

## Description
Connect your **Mabl** account to any AI agent and take full control of your AI-powered E2E testing and quality orchestration through natural conversation.

### What you can do

- **Plan Orchestration** — List all test plans and trigger immediate executions across specific environments (staging, production) directly from your agent
- **Execution Monitoring** — Track the real-time status of ongoing test runs and retrieve detailed outcome summaries including pass/fail rates and durations
- **AI Failure Analysis** — Deep-dive into execution results to extract precise failure reasons, diagnostic insights, and visual screenshots for rapid debugging
- **Environment Audit** — List configured testing environments and retrieve associated variables to ensure accurate test execution context
- **App & API Discovery** — Enumerate all monitored applications and their target URLs (web + API) to manage your testing grid securely
- **Label & Tag Management** — Discover and list plan labels used to group and trigger specific testing suites across your organization

### How it works

1. Subscribe to this server
2. Enter your Mabl API Key
3. Start managing your test automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Automation Engineers** — trigger complex test plans and analyze failure diagnostics through natural conversation without leaving your IDE
- **Software Developers** — verify build quality and retrieve session screenshots to debug UI regressions directly from your workspace
- **DevOps Teams** — audit CI/CD test results and monitor environment health across multiple Mabl projects efficiently


## Available Tools (10)
- **mb.list_apps**: Use this to lookup application details.

List all applications on Mabl. Mabl is an AI-powered E2E testing platform for web, mobile, and API testing with self-healing tests
- **mb.get_app**: Get full details of a Mabl application including name, description, targets (web URLs + API base URLs), and labels
- **mb.list_envs**: ). Returns env names, IDs, and environment variables.

List all environments on Mabl
- **mb.list_plans**: Returns plan names, statuses, triggers, and linked apps/envs.

List all test plans (run policies) on Mabl
- **mb.trigger_plan**: Trigger a Mabl plan run via deployment event
- **mb.list_executions**: List latest execution results on Mabl
- **mb.get_execution**: Get full details of a Mabl execution result including status, duration, test outcomes, failure analysis, and screenshots
- **mb.list_tests**: List all API tests on Mabl
- **mb.list_labels**: Returns label names and associated plan counts.

List all labels (tags) used in Mabl plans
- **mb.workspace_info**: Does not require args.

Get workspace info for the authenticated Mabl API key including workspace name, org, and key metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mabl (AI-Powered Test Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Mabl test plans"

**🤖 AI Agent:**
> I've found 4 test plans: 'Daily-Smoke-Test' (ID: plan-123), 'Checkout-Regression' (ID: plan-456), 'Login-Flow-Validation' (ID: plan-789), and 'API-Health-Check' (ID: plan-012). Which one would you like to trigger or inspect?

---

**👤 You:**
> "Trigger the 'Checkout-Regression' plan in the Staging environment"

**🤖 AI Agent:**
> Triggering test plan 'Checkout-Regression'… I've successfully started the run in your Staging environment. I'll monitor the progress and notify you once the execution is complete. Would you like the initial status report?

---

**👤 You:**
> "Show me the details for the last failed execution"

**🤖 AI Agent:**
> Retrieving the most recent failed execution… Run ID 'exec-98765' failed 12 minutes ago during the 'Add to Cart' step. The AI analysis suggests a 'Button not clickable' error due to a visual overlay. I can provide the direct screenshot link if you'd like.


## ❓ FAQ

**Q: Can I see exactly why a Mabl test failed using my agent?**
Yes. Use the `mb.get_execution` tool with a specific Execution ID. Your agent will retrieve deep diagnostic information, including the failure reason, test outcomes, and visual screenshots to help you identify UI regressions instantly.

**Q: How do I trigger a specific test plan through a conversation?**
The `mb.trigger_plan` tool allows your agent to start executions associated with a Plan ID or Label. You can also specify an optional Environment ID to target a specific stage (e.g., Staging vs Prod) for your automated tests.

**Q: Can my agent list all available testing environments in my account?**
Absolutely. Use the `mb.list_envs` tool to identify all configured environments. Your agent will report the environment names, IDs, and any associated environment variables defined in Mabl.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mabl-ai-powered-test-automation](https://vinkius.com/mcp/mabl-ai-powered-test-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mabl (AI-Powered Test Automation)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mabl-ai-powered-test-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mabl (AI-Powered Test Automation)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mabl-ai-powered-test-automation": {
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
