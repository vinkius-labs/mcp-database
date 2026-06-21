# AirOps MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airops)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airops-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airops-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **AirOps** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airops](https://vinkius.com/mcp/airops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
