# CrewAI Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crewai-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Orchestrate multi-agent workflows via CrewAI — list crews and agents, kickoff autonomous runs, and monitor task execution directly from any AI agent.

## Description
Connect your **CrewAI Platform** (AMP) account to any AI agent and take full control of your autonomous multi-agent orchestration through natural conversation.

### What you can do

- **Crew Management** — List all deployed multi-agent workflows and extract pure JSON blueprints mapping the complete agent graph topology
- **Autonomous Kickoffs** — Activate multi-agent processing immediately by triggering crews with dynamic JSON inputs to start complex workflows
- **Live Run Monitoring** — Retrieve disconnected physical states of active executions, tracking agents as they complete sequential or parallel tasks
- **Agent & Task Auditing** — Enumerate isolated role-playing agents and globally registered modular operations to verify backstories and expected outcomes
- **Execution Control** — Dispatch instant interrupt signals to hard-stop active runs and manage internal LLM context boundaries
- **Webhook Oversight** — Inspect exact validation criteria for async results and monitor where Crew outcomes post standard JSON boundaries

### How it works

1. Subscribe to this server
2. Enter your CrewAI Agent Token (found in the 'Status' tab of your Crew page in the AMP Dashboard)
3. Start orchestrating your autonomous agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Architects** — manage and monitor complex multi-agent graphs and verify agent role-playing backstories
- **Developers** — trigger autonomous workflows and retrieve task results directly from the IDE or chat
- **Product Teams** — quickly prototype and test agentic workflows using natural language inputs
- **DevOps Teams** — monitor active crew executions and manage webhook integrations across environments


## Available Tools (3)
- **get_inputs**: Identify bounded inputs required to kickoff a crew
- **get_status**: Retrieve explicit execution state tracing limits
- **kickoff_crew**: Provision a highly-available JSON Payload generating hard execution bindings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrewAI Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all crews in my account"

**🤖 AI Agent:**
> I found 3 crews: 'Market-Research-Team' (ID: crew_abc), 'Content-Creation-Squad' (ID: crew_def), and 'Data-Analysis-Group' (ID: crew_ghi). Which one would you like to inspect?

---

**👤 You:**
> "Kickoff crew 'crew_abc' with input: {'topic': 'AI Trends 2024'}"

**🤖 AI Agent:**
> Crew 'crew_abc' has been kicked off! New Run ID: 'run_123'. The agents are now starting their autonomous research on 'AI Trends 2024'. I can monitor the status for you.

---

**👤 You:**
> "What is the backstory of agent 'agent_789'?"

**🤖 AI Agent:**
> Retrieving agent details... Agent 'agent_789' is a 'Senior Research Analyst'. Backstory: 'Expert in gathering and synthesizing complex data from multiple sources to provide actionable insights.'


## ❓ FAQ

**Q: Can my agent kickoff a new CrewAI workflow?**
Yes. Use the 'kickoff_crew' tool. Provide the Crew ID and a JSON object with the required inputs. The agent will activate the multi-agent processing immediately, returning a run ID for tracking.

**Q: How do I monitor the progress of an active agent run?**
Use the 'get_run_status' tool with your Crew ID and Run ID. Your agent will grab the live execution state, showing you which agents are currently working and which tasks have been completed.

**Q: Can I cancel a running crew via the agent?**
Absolutely. The 'cancel_run' tool dispatches an instant interrupt signal to the CrewAI platform, hard-stopping active LLM contexts and terminating the execution flow immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crewai-platform](https://vinkius.com/mcp/crewai-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CrewAI Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crewai-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CrewAI Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crewai-platform": {
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
