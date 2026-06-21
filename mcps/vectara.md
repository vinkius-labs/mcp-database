# Vectara MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vectara)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vectara-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vectara-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Empower your agent with Vectara's RAG capabilities. Search corpora natively, execute grounded chats, and manage indexed datasets easily.

## Description
Connect your **Vectara** environment to any AI agent to unlock enterprise-grade Retrieval-Augmented Generation (RAG) and semantic search directly inside your conversational IDE or workspace.

### What you can do

- **Semantic Search** — Query your indexed private corpora naturally and return highly relevant, grounded documents without traditional keyword matching limitations.
- **Conversational RAG** — Execute fully-fledged interactive chats leveraging Vectara's backend to provide detailed, cited answers strictly based on your secure documents.
- **Corpus Management** — List all available data corpora, retrieve unique keys, and discover the shape of your indexed data environment on the fly.
- **Document Auditing** — Monitor specific document indexes within a corpus, verify correct ingestions, or permanently delete obsolete files avoiding polluted search results.

### How it works

1. Subscribe to this server
2. Enter your Vectara API Key and Customer ID
3. Start retrieving knowledge from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes an elite cognitive search gateway to all your internal data.

### Who is this for?

- **Software Engineers** — debug RAG implementation challenges by directly testing `query` responses via chat instead of writing disposable test scripts.
- **Data Engineers** — securely remove stale database context arrays manually inserted into Vectara via quick conversational text commands.
- **Product Leads** — ask questions against internal product manuals stored as a Vectara corpus without waiting for the frontend UI development.
- **Technical Writers** — locate specific passages traversing across thousands of embedded documents effortlessly leveraging contextual semantic queries.


## Available Tools
- **execute_rag_chat**: Provide corpus keys and the user query to get a summarized AI response with citations.

Executes a RAG-powered chat completion
- **delete_corpus_document**: This action is irreversible.

Permanently removes a document from a corpus
- **get_corpus_details**: Retrieves metadata and configuration for a specific corpus
- **list_chat_sessions**: Lists previous RAG chat sessions
- **list_corpora**: Lists all corpora (searchable datasets) in the Vectara account
- **list_corpus_documents**: Lists all indexed documents within a specific corpus
- **perform_semantic_search**: Provide one or more comma-separated corpus keys and the query text.

Executes a semantic search across one or more corpora


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vectara** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all configured knowledge corpora I have in Vectara."

**🤖 AI Agent:**
> We retrieved 3 existing corpora within your active Customer ID cluster: 
- 'HR Manuals' (Key: `cor-29x`)
- 'DevOps Runbooks' (Key: `cor-81a`)
- 'Helpcenter FAQs' (Key: `cor-03f`)
Would you like me to pull the total document count indexing actively inside 'DevOps Runbooks'?

---

**👤 You:**
> "Query corpus `cor-81a` for instructions on 'rolling back kubernetes pods' and show only the top 3 best matching results."

**🤖 AI Agent:**
> I've searched corpus `cor-81a`. Here are the top 3 semantic matches:

1. From 'infra-deploy.pdf' (Score 0.94): "To safely rollback a deployed k8s pod replica containing faulty image configs, use `kubectl rollout undo deployment/api-server`."
2. From 'incident-231.md' (Score 0.88): "During yesterday's P1, we reversed the pods deployment to stabilization tag v2.1.0 using standard rollback patterns..."
3. From 'onboarding.txt' (Score 0.76): "New engineers must verify staging before any manual pod cluster rollbacks occur in production environments..."

---

**👤 You:**
> "List all active chat context session IDs for the last week."

**🤖 AI Agent:**
> I've retrieved historical chat sessions. You have 2 sessions retained matching your request: `chat-89bf` (Initiated: Mon 14th) covering Corpus HR, and `chat-21zx` (Initiated: Wed 16th) heavily focused on developer queries. Do you want to see the sequence of turns for the DevOps troubleshooting session?


## Installation & Usage

To install and use the **Vectara** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vectara](https://vinkius.com/mcp/vectara)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
