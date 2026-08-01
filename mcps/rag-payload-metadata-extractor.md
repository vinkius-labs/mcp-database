# RAG Payload Metadata Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rag-payload-metadata-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [text-processing](../categories/text-processing.md)

Extracts metadata, structural markers, and efficiency metrics from RAG source documents using deterministic regex patterns.

## Description
The RAG Payload Metadata Extractor MCP server provides a specialized engine for parsing raw text from RAG (Retrieval-Augmented Generation) source documents. It uses deterministic regex patterns to identify key metadata components such as titles, URLs, dates, and authors within document headers. Beyond simple extraction, the server computes critical efficiency metrics, including the extraction success rate per document and the exact byte-size ratio of metadata versus core content (payload overhead). This allows developers to quantify 'context bloat'—the amount of non-informative structural data consuming the LLM context window. By utilizing tools like `extract_metadata` and `get_structural_summary`, you can audit large datasets for metadata integrity and optimize your RAG pipelines for maximum information density.


## Available Tools (3)
- **extract_markers**: Extract markdown structural markers from text
- **extract_metadata**: Extract metadata pairs from text using @key: value pattern
- **get_structural_summary**: Provide a structural summary of the text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RAG Payload Metadata Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the metadata from this text: '@title: Annual Report\n@author: Jane Doe\n@url: https://vinkius.com/docs\n\nThis is the content.'"

**🤖 AI Agent:**
> {"extractedTitle": "Annual Report", "extractedUrl": "https://vinkius.com/docs", "extractionSuccessRate": 0.5, "metadataByteSize": 45, "contentByteSize": 28}

---

**👤 You:**
> "Check the efficiency of these extraction results."

**🤖 AI Agent:**
> The average overhead percentage across the provided dataset is 12.5%, with a highest observed overhead ratio of 0.45.

---

**👤 You:**
> "Identify structural markers in this markdown snippet."

**🤖 AI Agent:**
> The scan identified the following markers: '#', '*', and '-'.


## ❓ FAQ

**Q: How does the extraction process work?**
The server uses deterministic regex patterns to scan the beginning of a document for specific markers like '@author:' or '@url:'. Because it is deterministic rather than probabilistic, it only identifies data that strictly adheres to your predefined structural templates.

**Q: What is 'payload overhead'?**
Payload overhead refers to the ratio of metadata bytes to the actual core content size. High overhead indicates that a significant portion of your LLM context window is being occupied by structural headers rather than useful information.

**Q: Can I use this to audit large datasets?**
Yes. By using the `extract_metadata` tool, you can process a collection of extraction results to identify exactly which documents are missing essential metadata headers.


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
