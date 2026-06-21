# CrewAI Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crewai-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crewai-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crewai-platform-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **CrewAI Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crewai-platform](https://vinkius.com/mcp/crewai-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
