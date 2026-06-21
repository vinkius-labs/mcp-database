# FlowiseAI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowiseai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flowiseai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flowiseai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Build LLM orchestration flows visually with a drag-and-drop interface for creating AI chatbots, agents, and RAG pipelines.

## Description
Connect your **FlowiseAI** (self-hosted) instance to any AI agent and take full control of your LLM orchestration and RAG workflows through natural conversation.

### What you can do

- **Prediction Orchestration** — Trigger specific chatflows and retrieve LLM-generated responses programmatically using natural language inputs
- **Chatflow Management** — List all orchestration flows and retrieve detailed technical structures and metadata to monitor your AI agents
- **Vector Intelligence** — Programmatically upsert documents or raw data into the vector stores linked to your chatflows to ensure high-fidelity context
- **Component Oversight** — Access server-wide credentials, custom tools, and global variables to manage your complete Flowise ecosystem
- **Operational Visibility** — Monitor user feedback, leads, and assistant profiles directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Enter your **Flowise Instance URL** and **API Key**
3. Start orchestrating your LLM flows from Claude, Cursor, or any MCP client

No more manual testing in the Flowise UI for every prediction. Your AI acts as your dedicated LLM operations and orchestration coordinator.

### Who is this for?

- **AI Developers** — instantly test and trigger complex orchestration flows using natural language queries
- **Data Engineers** — automate document ingestion into vector stores without leaving your workspace
- **Product Managers** — monitor chatflow performance and review captured leads through simple AI commands


## Available Tools
- **get_chatflow_details**: Get details for a specific chatflow
- **get_server_version**: Get Flowise server version
- **list_ai_assistants**: List OpenAI-style assistants
- **list_chatflows**: List all LLM orchestration flows
- **list_flowise_credentials**: List configured credentials
- **list_chat_feedback**: List user feedback for a chatflow
- **list_flow_leads**: List captured leads
- **list_marketplace_templates**: List chatflow templates
- **list_external_tools**: List custom tools
- **list_flow_variables**: List global variables
- **execute_chatflow_prediction**: Trigger an LLM flow prediction
- **upsert_vector_data**: Push data into a vector store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FlowiseAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my chatflows in Flowise."

**🤖 AI Agent:**
> I've retrieved your LLM flows. You have 3 active chatflows: 'Customer Support Bot' (ID: cf_1), 'RAG Assistant' (ID: cf_2), and 'Lead Generator' (ID: cf_3). Which one would you like to inspect?

---

**👤 You:**
> "Execute chatflow 'cf_1' with question: 'How do I reset my password?'"

**🤖 AI Agent:**
> Prediction complete! The bot responds: 'To reset your password, please go to the login screen and click on "Forgot Password". Check your email for further instructions.' Would you like to review the session memory?

---

**👤 You:**
> "Upsert this data into vector store for chatflow 'cf_2': [data]"

**🤖 AI Agent:**
> Data ingested! I've successfully pushed the documents to the vector store associated with chatflow 'cf_2'. The new context is now available for RAG-based predictions.


## Installation & Usage

To install and use the **FlowiseAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowiseai](https://vinkius.com/mcp/flowiseai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
