# Distance Metrics Engine MCP Server

Calculate mathematically perfect Cosine, Euclidean, Manhattan, and Chebyshev distances between high-dimensional vectors local. Essential for embedding comparisons.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/distance-metrics-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Distance Metrics Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/distance-metrics-engine](https://vinkius.com/mcp/distance-metrics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
