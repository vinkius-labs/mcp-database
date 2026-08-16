# Document Metadata Flattener MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/document-metadata-flattener)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [vector-databases](../categories/vector-databases.md)

Flattens nested JSON metadata into dot-notation keys for vector store compatibility.

## Description
This MCP server provides essential utilities to transform deeply nested JSON metadata structures into a flat, single-level dictionary. By converting hierarchical data into dot-notation (e.g., `parent.child`) and bracket-notation for arrays (e.g., `tags[0]`), it ensures compatibility with vector databases like Chroma and FAISS that require flat metadata for efficient filtering. Use `flatten_metadata` to perform the transformation, `validate_metadata_schema` to check nesting depth, or `get_metadata_summary` to analyze structural complexity.


## Available Tools (3)
- **flatten_metadata**: Converts a complex nested metadata object into a flat dictionary with dot/bracket notation keys
- **get_metadata_summary**: Provides a high-level statistical overview of a metadata object complexity
- **validate_metadata_schema**: Checks if a metadata object meets depth or structural constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Document Metadata Flattener** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Flatten this metadata: {"source": {"url": "https://example.com", "page": 1}, "tags": ["news", "tech"]}"

**🤖 AI Agent:**
> {"source.url": "https://example.com", "source.page": 1, "tags[0]": "news", "tags[1]": "tech"}

---

**👤 You:**
> "Check the complexity of this metadata object."

**🤖 AI Agent:**
> The metadata has a nesting complexity of 'moderate' with 5 leaf nodes and contains arrays.

---

**👤 You:**
> "Is this metadata object too deep for processing?"

**🤖 AI Agent:**
> The object is valid and meets the required depth constraints for processing.


## ❓ FAQ

**Q: Why do I need to flatten my metadata?**
Many vector databases, such as Chroma or FAISS, cannot filter based on nested JSON objects. Flattening converts these into a single level of keys, making them searchable.

**Q: How does the tool handle arrays?**
The tool uses bracket-notation for array elements. For example, an array at `tags` becomes `tags[0]`, `tags[1]`, etc.

**Q: What happens if there is a key collision?**
If two different paths result in the same flattened key, the tool detects the collision and prioritizes the first encountered value to prevent silent data loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/document-metadata-flattener](https://vinkius.com/ai-agent-connect/document-metadata-flattener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Document Metadata Flattener** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `document-metadata-flattener` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Document Metadata Flattener** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "document-metadata-flattener": {
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
