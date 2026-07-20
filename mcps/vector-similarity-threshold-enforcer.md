# Vector Similarity Threshold Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vector-similarity-threshold-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Compute exact vector similarity scores and enforce strict relevance thresholds for RAG pipelines.

## Description
This MCP server provides a deterministic gatekeeper for Retrieval-Augmented Generation (RAG) pipelines. It computes exact vector similarity scores using Cosine, Dot Product, and Euclidean metrics with IEEE 754 floating-point precision. By utilizing tools like `calculate_similarity`, `check_threshold_violation`, and `validate_vector_format`, AI agents can prevent 'garbage in, garbage out' scenarios by ensuring retrieved context meets a strict mathematical standard. It is ideal for high-precision retrieval tasks where even minor deviations in similarity can lead to hallucinations.


## Available Tools (3)
- **calculate_similarity**: Provide the metric type and an optional threshold.

Computes a specific similarity score between two vectors using a chosen metric
- **check_threshold_violation**: Identifies how far a score has fallen below the required standard
- **validate_vector_format**: Pre-flight check to ensure vectors are compatible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vector Similarity Threshold Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cosine similarity between [0.1, 0.2, 0.3] and [0.1, 0.2, 0.4]."

**🤖 AI Agent:**
> The cosine similarity score is approximately 0.996.

---

**👤 You:**
> "Check if a score of 0.72 violates a threshold of 0.75."

**🤖 AI Agent:**
> Yes, there is a violation with a severity score of 0.03.

---

**👤 You:**
> "Validate these vectors: [[1, 2], [1, 2, 3]]."

**🤖 AI Agent:**
> The validation failed because the vectors have different dimensions.


## ❓ FAQ

**Q: What metrics are supported for similarity calculation?**
The `calculate_similarity` tool supports Cosine, Dot Product, and Euclidean metrics.

**Q: How can I ensure my vectors are compatible before calculation?**
You should use the `validate_vector_format` tool to verify that all arrays have identical dimensions and contain only valid numbers.

**Q: What happens if a similarity score is below my required threshold?**
You can use `check_threshold_violation` to identify the exact severity of the violation and how far the score has fallen below your target.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vector-similarity-threshold-enforcer](https://vinkius.com/mcp/vector-similarity-threshold-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vector Similarity Threshold Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vector-similarity-threshold-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vector Similarity Threshold Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vector-similarity-threshold-enforcer": {
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
