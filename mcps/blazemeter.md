# BlazeMeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blazemeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Automate continuous performance testing via BlazeMeter — manage workspaces, trigger load tests, and analyze active run metrics securely via AI.

## Description
Connect your **BlazeMeter** API credentials to any AI agent and integrate enterprise load testing natively into your DevOps and QA workflows.

### What you can do

- **Infrastructure Management** — List thoroughly your bounded Workspaces, Projects, and structural user metadata.
- **Test Operations** — Discover configured JMeter definitions and dynamically start active cloud-based performance hosts to execute load scaling securely.
- **Live Run Monitoring** — Query the operational health of live "Master" runs, fetch precise throughput reports (p90/p99 KPIs), and monitor active limits.
- **Emergency Controls** — Forcefully shut down runaway active cloud connections to protect source architecture during testing.

### How it works

1. Subscribe to this server
2. Enter your BlazeMeter Key ID and Secret
3. Seamlessly control load testing arrays from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Site Reliability Engineers (SREs)** — trigger rapid baseline tests and monitor p99 health metrics dynamically without switching contexts.
- **QA Automation Teams** — query active JMeter testing structures securely via chat during CI/CD cycles.
- **DevOps Engineers** — abruptly stop rogue master runs securely via natural language, safely isolating operational networks.


## Available Tools (10)
- **list_workspaces**: Identify bounded Workspace records inside the Headless BlazeMeter Platform
- **list_projects**: Perform structural extraction of Projects bounded to a Workspace
- **list_tests**: Provision a highly-available JSON Payload extracting bound Tests
- **get_test**: Retrieve explicit configuration tracing an active Vault limit Test
- **start_test**: Irreversibly execute explicit load generation validations spanning rich metrics
- **list_masters**: Enumerate explicitly attached structured rules exporting active Master records
- **get_master**: Dispatch an automated validation check routing explicit Gateway run status
- **stop_master**: Identify precise active arrays spanning native Gateway shutdown logic
- **get_report**: Inspect deep internal arrays mitigating specific Plan Math Reports
- **get_user**: Identify precise active arrays spanning native Identity parsing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlazeMeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the performance testing projects inside Workspace ID `123456`."

**🤖 AI Agent:**
> I queried your BlazeMeter workspace. Here are the active projects discovered: 
- 'Core Backend API Stress' (ID: 9942)
- 'Frontend Cache Bypass Load' (ID: 9945).

---

**👤 You:**
> "Trigger a new execution for load Test ID `987654`."

**🤖 AI Agent:**
> Understood. I executed a `POST` operation onto `api/v4/tests/987654/start`. The BlazeMeter orchestration engines are now dynamically spinning up the performance nodes (Master ID: `m-11223`).

---

**👤 You:**
> "Stop the actively running Master test ID `m-11223` immediately."

**🤖 AI Agent:**
> Emergency stop validated. The REST sequence transmitted a shutdown instruction correctly severing connections and scaling down the Master load orchestrator (`m-11223`).


## ❓ FAQ

**Q: Can my agent actually start a cloud performance test orchestrating servers?**
Yes. By utilizing the 'start_test' tool paired with an active Test ID, your AI agent securely pulls levers directly on BlazeMeter's cloud infrastructure to provision load generation hosts without any required GUI interaction.

**Q: How do I check the live status of an active test run (Master)?**
You can instruct your agent to use the 'get_master' or 'get_report' tool. It strictly evaluates live Gateway stats, throughput rates, and p90 indicators dynamically reporting back.

**Q: Is there a way for the AI to forcefully kill a rogue load test?**
Absolutely. Your agent can execute the 'stop_master' mutation—which immediately severs the test execution pipeline and protects vulnerable origin servers from unplanned stress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blazemeter](https://vinkius.com/mcp/blazemeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlazeMeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blazemeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlazeMeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blazemeter": {
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
