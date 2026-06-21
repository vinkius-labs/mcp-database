# Gatling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gatling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage load testing via Gatling Enterprise — list and start simulations, monitor test runs and request stats, and handle generator pools directly from any AI agent.

## Description
Connect your **Gatling Enterprise** account to any AI agent and take full control of your performance testing and high-scale load simulation through natural conversation.

### What you can do

- **Simulation Orchestration** — List all Gatling simulations defining load scenarios and retrieve IDs, class names, and team associations natively
- **Live Test Execution** — Trigger new performance test runs on Gatling Enterprise infrastructure and retrieve unique run IDs flawlessly
- **Test Run Monitoring** — Track execution progress, statuses, and peak virtual user (VU) counts for ongoing or completed simulations synchronously
- **Detailed Stats Retrieval** — Access full run details including request statistics, error counts, and injection start/end times limitlessly
- **Team & Quota Oversight** — Enumerate teams registered in Gatling Enterprise and monitor member counts and credit quotas securely
- **Artifact Management** — List uploaded test packages and artifacts to verify versions and upload timestamps across your environment
- **Resource Pool Auditing** — Retrieve the list of load generator pools, identifying regions and instance counts to verify scaling capacity
- **Autonomous Aborting** — Stop all load generators for a running simulation immediately to manage system resources and prevent overruns

### How it works

1. Subscribe to this server
2. Enter your Gatling Enterprise API Token (found in Settings > API Tokens)
3. Start managing your load testing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance & QA Engineers** — trigger load tests and monitor simulation results without manual dashboard checks
- **SRE & DevOps Teams** — audit team quotas and verify load generator pool capacity using natural language
- **Developers** — test and debug performance scenario configurations and verify request stats in real-time
- **Ops Managers** — monitor virtual user peaks and credit consumption through the chat interface


## Available Tools (10)
- **list_simulations**: Simulations define load scenarios with VU populations. Returns names, IDs, class names, and team associations.

List all simulations on Gatling Enterprise
- **get_simulation**: Get full details of a Gatling simulation
- **start_simulation**: Returns run ID.

Start a Gatling simulation run
- **abort_simulation**: Abort a running Gatling simulation
- **list_runs**: List runs for a Gatling simulation
- **get_run**: Get full details of a Gatling run
- **list_teams**: List teams on Gatling Enterprise
- **list_packages**: List uploaded packages/artifacts on Gatling Enterprise
- **list_tokens**: List API tokens on Gatling Enterprise
- **list_pools**: List load generator pools on Gatling Enterprise


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gatling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all simulations on Gatling Enterprise"

**🤖 AI Agent:**
> Retrieving simulations... I found 3 active scenarios: 'User-Login-Stress-Test', 'Search-API-Performance', and 'Checkout-Flow-Baseline'. Which one would you like to start or view history for?

---

**👤 You:**
> "Start simulation 'abc-123'"

**🤖 AI Agent:**
> Simulation run started! I've triggered 'abc-123' on the Enterprise infrastructure. Your run ID is 'run_xyz789'. I'll monitor the progress and notify you when the virtual user peak is reached.

---

**👤 You:**
> "Show me the stats for run 'run_xyz789'"

**🤖 AI Agent:**
> Retrieving stats for run_xyz789... The test achieved a peak of 500 Virtual Users. Total requests: 12,500. Error rate: 0.05%. Average response time: 120ms. Would you like a breakdown by request type?


## ❓ FAQ

**Q: Can my agent start a Gatling simulation run via chat?**
Yes. Use the 'start_simulation' tool with the specific Simulation ID. The agent will command the Gatling Enterprise infrastructure to begin the load test and return a unique run ID for tracking.

**Q: How do I check the request statistics for a completed test run via chat?**
Use the 'get_run' tool. Provide the Run ID. Your agent will fetch the full details of the execution, including request stats, error counts, and the virtual user peak reached during the test.

**Q: Can I see my credit quotas and team member counts through the agent?**
Absolutely. Use the 'list_teams' tool. Your agent will enumerate the teams registered in your Gatling Enterprise account and monitor their member counts and available credit quotas natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatling](https://vinkius.com/mcp/gatling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gatling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gatling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gatling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gatling": {
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
