# BM25 Context Relevance Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bm25-context-relevance-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Deterministic BM25 relevance scoring engine for RAG optimization.

## Description
This MCP server provides a precision engine for calculating document relevance using the BM25 algorithm. It allows AI agents to solve the RAG relevance problem without relying on expensive LLM calls by providing deterministic, mathematical scores. Use `compute_relevance_score` to find how relevant a specific document is to a query, `calculate_term_weights` to compute term importance (IDF), and `analyze_document_composition` to extract structural statistics like token counts and frequencies.


## Available Tools (3)
- **analyze_document_composition**: Extracts statistics from a document
- **calculate_term_weights**: Computes the IDF for each term in a query
- **compute_relevance_score**: Calculates the BM25 relevance score for a document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BM25 Context Relevance Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the relevance score for a query 'apple' in a document containing 'apple pie' with a corpus size of 100, term doc counts {'apple': 10}, and avg doc length 50."

**🤖 AI Agent:**
> The calculated BM25 score for the document is approximately 1.45, indicating high relevance.

---

**👤 You:**
> "What is the IDF weight for the term 'algorithm' in a corpus of 500 documents where it appears in 50 documents?"

**🤖 AI Agent:**
> The calculated IDF weight for 'algorithm' is approximately 2.30.

---

**👤 You:**
> "Analyze the composition of this document: ['the', 'quick', 'brown', 'fox']"

**🤖 AI Agent:**
> The document length is 4 tokens, and the term frequency map is {'the': 1, 'quick': 1, 'brown': 1, 'fox': 1}.


## ❓ FAQ

**Q: How does the scoring work?**
The engine uses the BM25 algorithm, calculating IDF based on corpus size and term prevalence, then applying length normalization and saturation constants.

**Q: Do I need an LLM to calculate scores?**
No, this tool provides deterministic mathematical results using the `compute_relevance_score` function without any LLM involvement.

**Q: What inputs are required for scoring?**
You must provide query tokens, document tokens, corpus size, term document counts, and average document length.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bm25-context-relevance-scorer](https://vinkius.com/mcp/bm25-context-relevance-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BM25 Context Relevance Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bm25-context-relevance-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BM25 Context Relevance Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bm25-context-relevance-scorer": {
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
