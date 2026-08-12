# MinHash Text Deduplicator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/minhash-text-deduplicator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Detect near-duplicate texts using MinHash signatures and Jaccard similarity.

## Description
This MCP server provides tools to identify redundant content within large text collections. By using shingling and deterministic MinHash signatures, it estimates Jaccard similarity to find near-duplicates. Use `compute_similarity_matrix` to see how all texts relate, `identify_duplicate_clusters` to group similar items, or `check_is_duplicate` to verify if a specific text already exists in your library.


## Available Tools (3)
- **identify_duplicate_clusters**: Groups texts into distinct sets of near-duplicates based on a specific similarity requirement
- **check_is_duplicate**: Performs a binary check to determine if a new piece of text is a near-duplicate of any existing text
- **compute_similarity_matrix**: Calculates the estimated Jaccard similarity between all provided text entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MinHash Text Deduplicator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all groups of duplicate texts in this list: ['Hello world', 'Hello world!', 'Goodbye moon', 'Goodbye moon!'] with a threshold of 0.8."

**🤖 AI Agent:**
> [[0, 1], [2, 3]]

---

**👤 You:**
> "Is 'The quick brown fox' a duplicate of ['The quick brown fox jumps over the lazy dog'] with a threshold of 0.5?"

**🤖 AI Agent:**
> No, the similarity is below the threshold.

---

**👤 You:**
> "Show me the similarity matrix for these three sentences: ['A', 'B', 'C']."

**🤖 AI Agent:**
> [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]


## ❓ FAQ

**Q: How does the similarity estimation work?**
It uses MinHash signatures to estimate the Jaccard similarity between sets of shingles, providing a score between 0.0 and 1.0.

**Q: What is the purpose of the `ngramSize` parameter?**
The `ngramSize` determines the length of the shingles. A larger size requires more exact sequence matches to trigger a duplicate detection.

**Q: Can I use this to clean up my vector database?**
Yes, you can use `identify_duplicate_clusters` to find redundant entries and remove them to prevent bloat in your vector stores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/minhash-text-deduplicator](https://vinkius.com/mcp/minhash-text-deduplicator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MinHash Text Deduplicator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `minhash-text-deduplicator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MinHash Text Deduplicator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "minhash-text-deduplicator": {
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
