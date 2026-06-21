# Flowise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowise)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flowise-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flowise-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage low-code AI workflows via Flowise — run predictions, track chatflows and agentflows, handle tools, and audit execution history directly from any AI agent.

## Description
Connect your **FlowiseAI** instance to any AI agent and take full control of your low-code generative AI application development through natural conversation.

### What you can do

- **Chatflow Orchestration** — List and retrieve detailed architectural nodes and edges for all deployed Chatflows within your Flowise instance natively
- **Agentic Workflow Control** — Access compound Agentflows defining complex AI tasks and multi-step reasoning logic synchronously
- **Live AI Prediction** — Commands the backend to submit user questions to specific Chatflows and retrieve generated AI responses in real-time
- **Execution History Auditing** — Pull precise past execution traces and conversational logs to debug logic chains and monitor agent performance limitlessly
- **Tool & Integration Discovery** — Retrieve custom tools and third-party integrations configured in your Flowise environment to verify available capabilities
- **Credential Oversight** — Enumerate stored credential components used to authenticate your AI logic chains securely within the platform
- **System Health Monitoring** — Verify instance status and available base endpoints to ensure your AI orchestration layer is operational

### How it works

1. Subscribe to this server
2. Enter your Flowise Base URL and API Key (found in your Flowise Settings)
3. Start managing your AI workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug Chatflows and Agentflows without leaving the development environment
- **Automation Engineers** — trigger AI predictions and monitor execution histories using natural language
- **Product Teams** — audit available AI tools and verify conversational logs in real-time
- **Data Scientists** — evaluate different LLM orchestration patterns and logic chains through natural conversation


## Available Tools
- **list_chatflows**: List chatflows
- **get_chatflow**: Get chatflow details
- **predict**: Run prediction on chatflow
- **list_agentflows**: List agentflows
- **list_tools**: List available tools
- **list_credentials**: List credentials
- **get_history**: Get chat execution history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flowise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask chatflow 'abc-123': 'Summarize this document: [Context]'"

**🤖 AI Agent:**
> Prediction initiated! I've sent your request to Flowise chatflow abc-123. The AI response is: 'Based on the provided context, the document outlines three primary growth strategies for the next fiscal year...'

---

**👤 You:**
> "List all active chatflows in my instance"

**🤖 AI Agent:**
> Retrieving chatflows... I found 5 active flows: 'Customer Support Bot', 'RAG Knowledge Base', 'Legal Assistant', 'Lead Generator', and 'Developer Helper'. Which one would you like to explore?

---

**👤 You:**
> "Show me the execution history for chatflow 'Legal-Assistant'"

**🤖 AI Agent:**
> Retrieving history... For 'Legal-Assistant' (ID: 789), I found 10 recent executions. Highlights include a query about 'GDPR compliance' and another regarding 'Contract Review'. Would you like the logs for any of these?


## Installation & Usage

To install and use the **Flowise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowise](https://vinkius.com/mcp/flowise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
