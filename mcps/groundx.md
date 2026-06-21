# GroundX MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/groundx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/groundx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/groundx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Data search and RAG optimization platform.

## Description
The GroundX MCP server enables your AI agent to search across enterprise data stores and manage RAG (Retrieval-Augmented Generation) pipelines, retrieving highly relevant document chunks seamlessly.


## Available Tools
- **create_bucket**: Create a new bucket
- **create_group**: Create a new group
- **get_customer_info**: Retrieve account and customer details
- **get_ingest_status**: Check the processing status of an ingestion task
- **ingest_documents**: Ingest documents into GroundX from URLs or local paths
- **ingest_website**: Crawl and ingest content from a website URL
- **list_buckets**: List all buckets (containers for documents)
- **list_content**: List all ingested documents
- **list_groups**: List all groups (aggregations of buckets)
- **list_workflows**: List all RAG workflows
- **search_content**: Perform semantic search across all content
- **search_documents**: Search for specific documents based on metadata or content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GroundX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my GroundX data buckets."

**🤖 AI Agent:**
> You have 2 active buckets: 'Knowledge Base' (ID: 101) and 'Support Docs' (ID: 102).

---

**👤 You:**
> "Search for 'refund policy' in bucket 102."

**🤖 AI Agent:**
> According to the 'Support Docs', refunds are processed within 5-7 business days upon request.

---

**👤 You:**
> "Check the document count in bucket 101."

**🤖 AI Agent:**
> Bucket 101 ('Knowledge Base') currently contains 14,502 indexed documents.


## Installation & Usage

To install and use the **GroundX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/groundx](https://vinkius.com/mcp/groundx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
