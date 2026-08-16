# Retrieval Relevance Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/retrieval-relevance-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-processing](../categories/data-processing.md)

A deterministic scoring engine that filters retrieved documents using Jaccard, TF-IDF, and coverage metrics.

## Description
This MCP server provides a deterministic scoring engine to solve the noise and hallucination problems in RAG (Retrieval-Augmented Generation). It evaluates the relationship between a query and retrieved documents using three mathematical metrics: Jaccard Similarity for keyword overlap, TF-IDF Cosine Similarity for term importance, and Query Term Coverage for information density. Use `score_documents` to filter out irrelevant context, `get_scoring_config` to inspect weight distributions, or `analyze_coverage_gap` to diagnose why specific terms are missing from your retrieval set. It is designed to ensure only high-signal text reaches your AI client.


## Available Tools (3)
- **get_scoring_config**: Retrieves the current operational scoring parameters and weight distributions
- **analyze_coverage_gap**: Identifies which specific terms from a query are missing from the provided document set
- **score_documents**: Calculates relevance scores for a collection of documents against a single query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retrieval Relevance Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Score these documents for the query 'climate change impact on oceans': ['The oceans are warming due to climate change.', 'The weather is sunny today.']"

**🤖 AI Agent:**
> The first document has a high relevance score due to exact keyword overlap and coverage, while the second document is filtered out.

---

**👤 You:**
> "What are the default weights used by the engine?"

**🤖 AI Agent:**
> The default weights are 0.3 for keyword, 0.5 for tfidf, and 0.2 for coverage.

---

**👤 You:**
> "Check if the term 'photosynthesis' is present in my documents."

**🤖 AI Agent:**
> The term 'photosynthesis' is missing from the provided document set.


## ❓ FAQ

**Q: How does the scoring work?**
The engine calculates a composite score by combining Jaccard similarity, TF-IDF cosine similarity, and query term coverage using configurable weights.

**Q: Can I customize the weights?**
Yes, you can pass a custom weights object to the `score_documents` tool to prioritize different metrics like keyword overlap or TF-IDF.

**Q: How do I diagnose why a document was filtered out?**
You can use the `analyze_coverage_gap` tool to identify which specific terms from your query are missing from the retrieved documents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/retrieval-relevance-scorer](https://vinkius.com/ai-agent-connect/retrieval-relevance-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retrieval Relevance Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `retrieval-relevance-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retrieval Relevance Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retrieval-relevance-scorer": {
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
