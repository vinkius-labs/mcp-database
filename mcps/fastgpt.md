# FastGPT MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fastgpt)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fastgpt-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fastgpt-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage FastGPT Knowledge Bases — automate dataset creation, document ingestion, and RAG search directly from any AI agent.

## Description
Connect your AI workflows to **FastGPT**, the powerful open-source platform for building knowledge-based AI applications. This MCP provides 12 tools for full lifecycle management of datasets, apps, and RAG (Retrieval-Augmented Generation) pipelines.

### What you can do

- **Dataset Orchestration** — Create, list, and manage knowledge base datasets with granular control over configurations
- **Document Ingestion** — Push text content or chunks directly to datasets for automatic indexing and vectorization
- **Semantic Search** — Run advanced semantic queries against your knowledge bases to test relevance and RAG quality
- **Application Management** — List and inspect AI applications to monitor their configurations and linked datasets
- **OpenAI-Compatible Chat** — Trigger RAG-powered chat completions with full context, session tracking, and intermediate step visibility

### How it works

1. Subscribe to this server
2. Set up [**FastGPT**](https://fastgpt.in/) (cloud or self-hosted)
3. Navigate to your **App** settings and enter the **API Access** section
4. Generate an **API Key**
5. Identify your **Base URL** (e.g., `https://api.fastgpt.in` for cloud)
6. Insert both into the fields below to start managing your RAG pipelines.

### Who is this for?

- **Knowledge Engineers** — automate the ingestion of documentation across multiple datasets
- **RAG Developers** — debug semantic search results and optimize chunking strategies programmatically
- **System Integrators** — build complex AI workflows that require dynamic knowledge base management


## Available Tools
- **chat_completions**: Supports chatId for context tracking, streaming, and detailed intermediate steps.

Send a message to a FastGPT application
- **get_embeddings**: Useful for semantic search outside of FastGPT.

Generate text embeddings
- **get_app_detail**: Get details for a specific AI application
- **get_dataset_detail**: Get details for a specific dataset
- **create_dataset**: Create a new dataset (knowledge base)
- **delete_dataset_data**: Delete specific data from a dataset
- **list_apps**: List AI applications
- **list_dataset_data**: List data items in a dataset
- **list_datasets**: Can filter by parentId or search keyword.

List knowledge base datasets
- **push_dataset_data**: Add or update data in a dataset
- **search_dataset_data**: Perform semantic search on a dataset
- **update_dataset_data**: Update existing data in a dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FastGPT** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AI applications in FastGPT."

**🤖 AI Agent:**
> I've retrieved your applications. You have 2 active apps: 'Customer Support' (ID: app_1) and 'Internal HR' (ID: app_2). Which one would you like to inspect?

---

**👤 You:**
> "Search dataset 'ds_123' for 'company refund policy'."

**🤖 AI Agent:**
> Searching dataset 'ds_123'... I found 2 relevant results: 1. 'Refunds are processed in 5 days' (Score: 0.95), 2. 'Request via portal' (Score: 0.88). Would you like to see the full content?

---

**👤 You:**
> "Create a new dataset named 'Internal Documentation'."

**🤖 AI Agent:**
> Creating dataset... 'Internal Documentation' has been created successfully. ID: `ds_docs_999`. You can now start pushing data to it using the `push_dataset_data` tool.


## Installation & Usage

To install and use the **FastGPT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fastgpt](https://vinkius.com/mcp/fastgpt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
