# Embedding Similarity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/embedding-similarity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate mathematical distances and similarity scores between multidimensional numerical vectors.

## Description
The Embedding Similarity Calculator provides precise mathematical computations for comparing multidimensional vectors. Using tools like `compute_pairwise_metrics`, you can determine cosine similarity, Euclidean distance, dot product, and Manhattan distance between pairs. The `rank_vectors_by_metric` tool allows you to search through large sets of candidate vectors by finding the most similar or closest entries based on your chosen metric. Additionally, `validate_vector_dimensions` ensures that all vectors in a collection are mathematically compatible for group operations.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Embedding Similarity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cosine similarity between [1, 0] and [0, 1]?"

**🤖 AI Agent:**
> The cosine similarity between the two vectors is 0.0.

---

**👤 You:**
> "Rank these vectors by Euclidean distance to [0, 0]: [[1, 1], [2, 2], [0.5, 0.5]]"

**🤖 AI Agent:**
> [0.5, 0.5] is the closest vector with a distance of approximately 0.707, followed by [1, 1] and [2, 2].

---

**👤 You:**
> "Are these vectors compatible: [[1, 2], [1, 2, 3]]?"

**🤖 AI Agent:**
> No, the vectors are not compatible because they have different dimensions (2 and 3).


## ❓ FAQ

**Q: What metrics are supported?**
The calculator supports Cosine Similarity, Euclidean Distance, Dot Product Similarity, and Manhattan Distance. Tools available: `your_tool_name`.

**Q: Do all vectors need to have the same size?**
Yes, for any mathematical comparison to be valid, all vectors involved must share the exact same dimensionality.

**Q: How does ranking work for distance metrics?**
For distance-based metrics like Euclidean and Manhattan, vectors with smaller values are ranked higher. For similarity-based metrics like Cosine and Dot Product, larger values are ranked higher.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/embedding-similarity-calculator](https://vinkius.com/mcp/embedding-similarity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Embedding Similarity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `embedding-similarity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Embedding Similarity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "embedding-similarity-calculator": {
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
