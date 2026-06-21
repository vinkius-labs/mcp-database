# GroundX MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/groundx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Data search and RAG optimization platform.

## Description
The GroundX MCP server enables your AI agent to search across enterprise data stores and manage RAG (Retrieval-Augmented Generation) pipelines, retrieving highly relevant document chunks seamlessly.


## Available Tools (12)
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


## ❓ FAQ

**Q: How do I query my indexed documents?**
Simply ask the AI agent to search for a specific term or concept, and it will query the GroundX API to retrieve the most relevant textual chunks.

**Q: Can I manage data buckets from the agent?**
Yes, you can list your active buckets, check their document count, and verify index status.

**Q: Does it support adding new files to a bucket?**
Currently, the integration focuses on querying the optimized indexes. File ingestion should be managed through the GroundX dashboard or a separate pipeline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/groundx](https://vinkius.com/mcp/groundx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GroundX** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groundx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GroundX** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groundx": {
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
