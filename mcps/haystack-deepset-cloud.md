# Haystack (deepset Cloud) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/haystack-deepset-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/haystack-deepset-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/haystack-deepset-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Build and manage AI-powered search and RAG pipelines via deepset Cloud — search documents, run pipelines, and manage workspaces.

## Description
Connect your **deepset Cloud** account to any AI agent and manage your Haystack-powered RAG pipelines through natural conversation.

### What you can do

- **Workspaces** — List and manage isolated environments for different search contexts
- **Pipelines** — Visualize NLP topologies, including embedding nodes and retriever logic
- **Run Search** — Dispatch immediate LLM or Retriever invocations to test RAG pipelines
- **Document Management** — List files and inspect metadata attached to source document embeddings
- **Vector Search** — Trigger dense or sparse vector searches over indexed enterprise knowledge

### How it works

1. Subscribe to this server
2. Enter your deepset Cloud API URL and API Key
3. Start managing your AI pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI/ML Teams** — quickly audit pipeline configurations and test search results
- **RAG Developers** — integrate enterprise knowledge bases with AI agents for contextual answers
- **Product Managers** — monitor search performance and verify document indexing status


## Available Tools
- **list_workspaces**: List workspaces
- **list_pipelines**: List pipelines
- **get_pipeline**: Get pipeline details
- **run_pipeline**: Run a pipeline search
- **list_files**: List uploaded files
- **get_file**: Get file metadata
- **search_documents**: Search documents in index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Haystack (deepset Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pipelines in my 'production' workspace"

**🤖 AI Agent:**
> I found 3 pipelines in your production workspace: 'default-rag', 'semantic-search', and 'hybrid-retriever'. Which one would you like to inspect?

---

**👤 You:**
> "Run a search for 'AI security compliance' using the default-rag pipeline"

**🤖 AI Agent:**
> Running search… Based on your indexed documents, I found 5 relevant snippets. The main compliance requirements are… [results summary]. Would you like to see the source file IDs?

---

**👤 You:**
> "List the files in my 'knowledge-base' workspace"

**🤖 AI Agent:**
> You have 12 files in the 'knowledge-base' workspace. Recent uploads include 'q4_report.pdf', 'security_guidelines.md', and 'api_docs.txt'. I can fetch metadata for any of these files.


## Installation & Usage

To install and use the **Haystack (deepset Cloud)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/haystack-deepset-cloud](https://vinkius.com/mcp/haystack-deepset-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
