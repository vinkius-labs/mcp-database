# Cognee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cognee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cognee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cognee-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Build knowledge graphs from unstructured data — ingest text, extract entities and relationships, and search with graph-aware AI reasoning.

## Description
Connect your AI agent to **Cognee** — the open-source knowledge graph platform that transforms unstructured data into structured, searchable knowledge.

### What you can do

- **Add Data** — Ingest raw text, documents, or structured data into named datasets. Cognee processes and stores the data for subsequent graph construction
- **Cognify** — Transform ingested data into a structured knowledge graph by automatically extracting entities, relationships, and semantic connections
- **Search Knowledge** — Query the knowledge graph using four retrieval strategies: graph-aware completion (LLM + graph traversal), summaries, structured insights, or raw vector similarity
- **Get Insights** — Retrieve structured entity relationships showing how concepts connect across your knowledge base

### How it works

1. Subscribe to this server
2. Enter your Cognee API key
3. Ingest data → Cognify → Search with graph-aware reasoning

### Why Cognee over standard RAG?

- **Relationship-aware** — understands HOW facts connect, not just what they say
- **Graph + Vector hybrid** — combines graph traversal with semantic search for superior recall
- **Temporal awareness** — tracks when facts were added and reason over time-based connections


## Available Tools
- **cognee_add_data**: After ingestion, use the cognify tool to process the data into a structured knowledge graph with entities and relationships.

Ingest text or documents into the Cognee knowledge base. This is the first step before building a knowledge graph
- **cognee_cognify**: This step extracts entities, identifies relationships, generates embeddings, and creates the graph structure needed for intelligent search.

Process ingested data into a structured knowledge graph. Extracts entities, relationships, and builds a searchable graph structure
- **cognee_get_insights**: Useful for understanding relationships between topics, discovering hidden connections, and building comprehensive knowledge views.

Retrieve structured entity relationships and insights from the knowledge graph
- **cognee_search**: Search the knowledge graph using natural language. Returns context-aware answers using graph traversal and semantic search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cognee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add this research data to my knowledge base: 'Transformer models were introduced by Vaswani et al. in 2017 in the paper Attention Is All You Need. They use self-attention mechanisms and have become the foundation for models like GPT, BERT, and T5.'"

**🤖 AI Agent:**
> Data ingested successfully!

**[ingested]** | Dataset: default
> Transformer models were introduced by Vaswani et al. in 2017...

📎 Data added to dataset 'default'. Run cognify to process into knowledge graph.

---

**👤 You:**
> "Process my data into a knowledge graph."

**🤖 AI Agent:**
> Knowledge graph processing started!

**[cognify]** | Dataset: default
> Extracted entities: Transformer, Vaswani, GPT, BERT, T5, self-attention
> Relationships: introduced_by, foundation_for, uses_mechanism
> Status: processing

---

**👤 You:**
> "What is the relationship between Transformers and GPT?"

**🤖 AI Agent:**
> Graph-aware answer:

> Transformers are the foundational architecture for GPT models. Introduced by Vaswani et al. in 2017, the Transformer architecture uses self-attention mechanisms. GPT (Generative Pre-trained Transformer) builds upon this architecture for autoregressive language modeling.

Relationships found:
- Transformer → foundation_for → GPT
- Transformer → uses → self-attention
- Transformer → introduced_by → Vaswani et al.


## Installation & Usage

To install and use the **Cognee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cognee](https://vinkius.com/mcp/cognee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
