# AirOps MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airops)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI workflow orchestration — execute models, manage agents, and query memory via AI.

## Description
Connect your **AirOps** account to your AI agent to unlock professional AI workflow orchestration and agent management. From executing complex multi-step workflows synchronously or asynchronously to interacting with specialized chat agents and managing managed memory stores, your agent handles your AI operations through natural conversation.

### What you can do

- **Workflow Orchestration** — Execute and monitor AirOps apps and workflows, passing custom parameters and retrieving structured results
- **Agent Interaction** — Chat directly with your specialized AirOps agents to perform niche tasks or leverage unique agent instructions
- **Memory Management** — Search within managed memory stores (vector databases) and add documents to enrich your AI's domain knowledge
- **File Orchestration** — Upload and manage files to be used as inputs for your AI workflows and data extraction tasks
- **Real-time Status** — Monitor execution statuses and cancel long-running AI tasks directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AirOps API Key
3. Start executing workflows and managing your AI assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — automate the execution of complex LLM chains and monitor performance effortlessly
- **Product Managers** — audit AI app outputs and manage specialized agent configurations on the fly
- **Operations Leads** — integrate AI-driven data extraction and analysis into existing business processes
- **Data Specialists** — manage and search internal knowledge bases using AirOps memory stores


## Available Tools (10)
- **upload_file**: Upload file for AI
- **list_apps**: List AI applications
- **get_app_details**: Get app metadata
- **execute_workflow_sync**: Best for quick tasks.

Run workflow synchronously
- **execute_workflow_async**: Run workflow asynchronously
- **get_execution_status**: Check execution progress
- **cancel_execution**: Stop a running task
- **chat_with_agent**: Interact with AI agent
- **search_memory_store**: Search vector database
- **add_memory_document**: Enrich AI knowledge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AirOps** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all AI apps in my AirOps workspace."

**🤖 AI Agent:**
> I've retrieved your apps. You have 12 active AirOps applications, including 'Content Summarizer', 'Data Extractor v2', and 'Legal Assistant'. Would you like the technical details for any of them?

---

**👤 You:**
> "Execute the 'Data Extractor' app (UUID: abc-123) with input 'Extract names from this text: John Doe visited London'."

**🤖 AI Agent:**
> I've executed the workflow. The AI has processed your request and returned the following structured data: { "names": ["John Doe"], "locations": ["London"] }. Would you like to save this result to a document?

---

**👤 You:**
> "Search my 'Knowledge Base' memory store for 'API integration guides'."

**🤖 AI Agent:**
> I've searched the 'Knowledge Base' memory store. I found 2 relevant document snippets discussing REST API authentication and Webhook setup. Would you like me to summarize these guides for you?


## ❓ FAQ

**Q: How do I find my AirOps API Key?**
Log in to your AirOps account, navigate to **Workspace Settings**, and look for the **API Keys** section. You can generate and copy your secure bearer token there.

**Q: What is the difference between synchronous and asynchronous execution?**
Synchronous execution (`execute_workflow_sync`) keeps the connection open until the AI finishes. Asynchronous (`execute_workflow_async`) returns an ID immediately, allowing you to check the status later, which is better for long-running tasks.

**Q: Can I search through my uploaded documents?**
Yes! Use the `search_memory_store` tool. It performs a semantic search across your managed memory stores, returning the most relevant document chunks for your query.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airops](https://vinkius.com/mcp/airops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AirOps** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AirOps** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airops": {
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
