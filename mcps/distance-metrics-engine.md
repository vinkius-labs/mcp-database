# Distance Metrics Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/distance-metrics-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/distance-metrics-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/distance-metrics-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate mathematically perfect Cosine, Euclidean, Manhattan, and Chebyshev distances between high-dimensional vectors local. Essential for embedding comparisons.

## Description
When working with embeddings in machine learning, calculating the Cosine Similarity between two 1024-dimensional vectors is a fundamental task. LLMs cannot perform this calculation accurately — they will approximate and get it wrong.

This MCP delegates the vector math to `ml-distance` locally, allowing the AI to perfectly compute similarity and distance metrics without cloud-API dependencies or math hallucinations.

### The Superpowers

- **Zero Hallucination:** Exact vector distances computed locally by your CPU.
- **Full Metric Suite:** Cosine, Euclidean, Manhattan, and Chebyshev distances with both distance and similarity values.
- **High-Dimensional Support:** Handles 1536-dimensional OpenAI embeddings in milliseconds.
- **Data Privacy:** Your embedding vectors and model weights never leave your machine.


## Available Tools
- **distance_metrics_calculate**: Calculate exact distances (Cosine, Euclidean, Manhattan) between high-dimensional vectors/embeddings offline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Distance Metrics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Cosine similarity between these two embedding vectors."

**🤖 AI Agent:**
> The exact cosine similarity is 0.9412, meaning the two documents are highly semantically similar. The cosine distance is 0.0588.

---

**👤 You:**
> "What is the Euclidean distance between [1, 2, 3] and [4, 5, 6]?"

**🤖 AI Agent:**
> The exact Euclidean distance is 5.196152. The corresponding similarity score (1/(1+d)) is 0.161290.

---

**👤 You:**
> "Measure the Manhattan distance between the user's feature vector and the cluster centroid."

**🤖 AI Agent:**
> The Manhattan distance computation returned exactly 12.0. This positions the user in the outer boundary of Cluster 3.


## Installation & Usage

To install and use the **Distance Metrics Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/distance-metrics-engine](https://vinkius.com/mcp/distance-metrics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
