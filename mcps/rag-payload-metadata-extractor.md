# RAG Payload Metadata Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rag-payload-metadata-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Extracts metadata and calculates data density for RAG source documents.

## Description
This MCP server provides deterministic tools to validate the structural integrity of RAG source documents. It uses strict pattern matching to identify metadata like Title, URL, Date, and Author. Use `extract_document_metadata` to pull specific fields, `calculate_size_metrics` to compare metadata byte size against core content, and `audit_document_integrity` to determine if a document is fit for RAG ingestion based on its header validity and success rate.


## Available Tools (3)
- **audit_document_integrity**: Provide a high-level summary of whether a document is fit for RAG ingestion
- **calculate_size_metrics**: Quantify the data distribution between metadata and the core body of a document
- **extract_document_metadata**: Extract specific metadata fields from a raw document string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RAG Payload Metadata Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you extract the metadata from this document: 'Title: Report A, URL: https://a.com, Date: 2023, Author: John'?"

**🤖 AI Agent:**
> The extracted metadata includes Title: Report A, URL: https://a.com, Date: 2023, and Author: John.

---

**👤 You:**
> "Is this document suitable for RAG ingestion?"

**🤖 AI Agent:**
> The document is fit for RAG ingestion as it contains a valid header and all required metadata fields were successfully identified.

---

**👤 You:**
> "What is the metadata to content ratio for this file?"

**🤖 AI Agent:**
> The metadata occupies 120 bytes, while the core content occupies 1500 bytes, resulting in a ratio of 0.08.


## ❓ FAQ

**Q: How does the extraction process work?**
The server uses deterministic regex patterns to identify metadata keys within a document's header. You can use `extract_document_metadata` to retrieve these fields.

**Q: What defines a document as fit for RAG?**
A document is considered fit for RAG if it has a valid metadata header and a 100% success rate in field extraction, as verified by `audit_document_integrity`.

**Q: Can I measure the density of my document metadata?**
Yes, the `calculate_size_metrics` tool provides the byte-size ratio between the extracted metadata and the core document content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rag-payload-metadata-extractor](https://vinkius.com/mcp/rag-payload-metadata-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RAG Payload Metadata Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rag-payload-metadata-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RAG Payload Metadata Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rag-payload-metadata-extractor": {
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
