# FastGPT MCP Server

Manage FastGPT Knowledge Bases — automate dataset creation, document ingestion, and RAG search directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fastgpt)

## Overview
**Category:** data-management
**Tools Count:** 12

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


## Installation & Usage

To install and use the **FastGPT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fastgpt](https://vinkius.com/mcp/fastgpt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
