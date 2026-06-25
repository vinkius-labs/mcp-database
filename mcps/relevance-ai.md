# Relevance AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/relevance-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Automate autonomous AI agents via Relevance AI — manage tools, trigger tasks, and monitor results directly.

## Description
Connect your **Relevance AI** account to any AI agent and take full control of your autonomous AI workforce and tool orchestration through natural conversation. Relevance AI provides a world-class platform for building and scaling multi-agent systems, and this integration allows you to trigger autonomous agents, execute custom studios (tools), and monitor long-running task histories directly from your chat interface.

### What you can do

- **Agent & Workforce Orchestration** — List all available autonomous agents and trigger them to perform specific goals with dynamic inputs programmatically.
- **Studio & Tool Intelligence** — Access and monitor your custom AI 'Studios' and execute them with complex parameters directly from the AI interface.
- **Task Lifecycle Management** — Retrieve real-time progress for background tasks and monitor final outputs to ensure your autonomous workflows are always synchronized.
- **Knowledge & RAG Control** — List and search through your agent's knowledge base items and datasets via natural language.
- **Operational Monitoring** — Track system activity and manage regional deployments using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Relevance AI Region Code (e.g., bcbe5a) and API Key
3. Start managing your autonomous AI teams from Claude, Cursor, or any MCP-compatible client

No more manual dashboard refreshing for task results. Your AI acts as a dedicated orchestrator for your entire agentic infrastructure.

### Who is this for?

- **AI Operations Managers** — quickly retrieve task summaries and monitor agent deployments without switching tabs.
- **Automation Engineers** — automate the triggering of complex multi-agent workflows via natural conversation.
- **Developers** — integrate real-time task results and studio execution into custom business architectures.


## Available Tools (11)
- **delete_task**: Permanently delete a task record
- **get_agent_details**: Get metadata for an agent
- **get_task_status**: Check status and results of a task
- **list_agents**: List all AI agents
- **get_knowledge**: Get details for a knowledge base
- **list_executions**: List all agent execution history
- **list_knowledge_items**: List knowledge base items
- **list_agent_tasks**: List recent agent tasks
- **trigger_agent**: Start an agent task
- **trigger_tool**: Execute a specific tool (Studio)
- **list_tools**: List all studios/tools


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relevance AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available autonomous agents."

**🤖 AI Agent:**
> I've retrieved your agents. You have 3 active personas: 'Market Researcher', 'Data Analyst', and 'Sales Lead'. Which one would you like to trigger?

---

**👤 You:**
> "Show me all AI agents in my workspace with their execution statistics from the last 7 days."

**🤖 AI Agent:**
> 6 AI agents in your workspace. "Customer Support Agent" ran 1,234 tasks (98.2% success rate, avg 3.4s response time). "Lead Qualifier" processed 567 leads (87% accuracy on scoring). "Content Writer" generated 89 articles (avg quality score: 8.4/10). "Data Analyst" executed 234 queries. "Email Responder" handled 456 emails. "Research Agent" completed 78 deep research tasks. Total executions: 2,658. Total tokens used: 4.2M. Cost: $84.60.

---

**👤 You:**
> "Trigger the Lead Qualifier agent to analyze and score a batch of 50 new inbound leads."

**🤖 AI Agent:**
> Lead Qualifier agent triggered for batch processing. 50 leads submitted for analysis. Processing status: 34 completed, 16 in queue. Results so far: 8 scored as Hot (80-100), 14 as Warm (50-79), 12 as Cold (below 50). Top lead: Sarah Chen from Meridian Corp (score: 96, enterprise budget confirmed, immediate need). 3 leads flagged for manual review due to incomplete data. Estimated completion: 2 minutes. Results will be synced to your CRM automatically.


## ❓ FAQ

**Q: Can my AI automatically trigger another autonomous agent in Relevance AI?**
Yes! Use the `trigger_agent` tool. Provide the `agent_id` and the user message/goal, and your agent will initiate the autonomous workflow in your Relevance account instantly.

**Q: How do I find my Region Code and API Key?**
The Region Code is in your dashboard URL (e.g., `bcbe5a`). For the API Key, log in to Relevance AI, navigate to **Settings** > **API Keys**, and generate a new secret key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/relevance-ai](https://vinkius.com/mcp/relevance-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relevance AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relevance-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relevance AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relevance-ai": {
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
