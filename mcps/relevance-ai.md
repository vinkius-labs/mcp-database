# Relevance AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/relevance-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Equip your AI to trigger custom autonomous agents, execute chained prompts, and manage unstructured knowledge datasets directly within your Relevance AI studio.

## Description
Connect your conversational AI to your **Relevance AI** workspace. By wrapping your custom agents, datasets, and API tools into this MCP extension, you transform your chat interface into a command center for orchestrating complex, autonomous AI operations and large-scale data workflows.

### What you can do

- **Orchestrate Agents** — Command your pre-built autonomous agents to execute tasks (`trigger_agent`). Monitor their progress and read their exact reasoning steps dynamically (`get_agent_run`). Use `list_agents` to discover all available AI worker configurations.
- **Execute Tasks & Workflows** — Trigger predefined chained prompts or specific micro-tasks without leaving your chat (`trigger_task`), scaling repetitive workflows reliably.
- **Manage Knowledge Datasets** — Take full control of your vector databases and tables. Insert new rows of knowledge directly from conversational context (`insert_documents`), retrieve raw unstructured data entries (`get_documents`), or surgically delete obsolete knowledge base items (`delete_documents`).

### How it works

1. Add the Relevance AI extension to your MCP hub.
2. Supply your `Project ID`, `API Key`, and your assigned `Region` (e.g., "us-east-1" or "v2") from your Relevance AI settings.
3. Prompt your assistant: "Trigger the 'Lead Research' agent with the company name 'Google' and monitor the run until completion. Then, insert the output directly into our 'competitors' dataset."

### Who is this for?

- **AI Engineers & Builders** — Run end-to-end tests on your chained logic and customized agents directly from your terminal or chat without touching the studio GUI.
- **Data Analysts** — Move processed insights, raw texts, and structured metadata into Relevance AI datasets using natural language.
- **Operations Teams** — Combine the output of your everyday AI chat intimately with your specialized Relevance AI autonomous agents for highly productive compounding workflows.


## Available Tools
- **delete_documents**: This action is irreversible.

Deletes documents from a dataset by their IDs
- **list_tasks**: Lists all tasks (chained prompts) in the studio
- **list_tools**: Lists all custom tools registered in the studio
- **trigger_agent**: Provide inputs as a JSON object.

Triggers an AI agent execution
- **trigger_task**: Triggers a specific task execution
- **get_agent_run**: Retrieves the status and logs of a specific agent run
- **get_documents**: Retrieves documents from a dataset
- **insert_documents**: Provide documents as a JSON array of objects.

Inserts documents into a dataset
- **list_agents**: Lists all AI agents in the Relevance AI studio
- **list_datasets**: Lists all datasets (knowledge tables) in the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relevance AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available agents in my Relevance AI Studio and their IDs."

**🤖 AI Agent:**
> I executed `list_agents` and retrieved your available agents: 1. "Sales SDR Bot" (ID: ag-3j92...), 2. "Researcher Assistant" (ID: ag-4m91...). You can trigger either one anytime by using its specific ID.

---

**👤 You:**
> "Start a run for the 'Market Analysis' agent passing `{"company": "OpenAI"}` as the payload, then tell me the Run ID."

**🤖 AI Agent:**
> I successfully initiated the agent using `trigger_agent`. The execution process has started. Your tracked Run ID is `rn-92f7a4`. Would you like me to ping its progress using `get_agent_run`?

---

**👤 You:**
> "Insert this JSON array of top competitor articles into the 'competitor_docs' dataset."

**🤖 AI Agent:**
> I invoked `insert_documents` targeting dataset 'competitor_docs' with your provided dataset rows. The array of records has been persistently saved into your Relevance AI knowledge table.


## ❓ FAQ

**Q: Can the agent monitor a long-running relevance AI agent task?**
Yes. You can trigger an agent using `trigger_agent`, and because it provides a `run_id`, you can explicitly prompt your local Assistant to periodically "check in on the status using `get_agent_run` every minute until finished" or ask it to summarize the step-by-step agent logs after completion.

**Q: What is the differences between tasks, tools, and agents in Relevance AI?**
Agents are autonomous workers capable of making step-by-step reasoning choices based on instructions and tools. Tasks are linear, pre-chained sets of commands and prompts. Tools (`list_tools`) are the individual capabilities, like a custom API integration or web scraper, that tasks and agents utilize to perform their actions.

**Q: How do I find my specific Region and Project ID?**
These details are typically nested within the URL string when you are logged into your workspace or found globally in your developer API keys configuration pane inside your Relevance AI team dashboard. The Region is usually something like 'us-east-1' or 'v2'.


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
3. Set Type to "SSE", enter `relevance-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
