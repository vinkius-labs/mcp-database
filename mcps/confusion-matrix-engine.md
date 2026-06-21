# Confusion Matrix Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/confusion-matrix-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/confusion-matrix-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/confusion-matrix-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministically calculate True Positives, FP, Precision, Recall, F1-Score, and Accuracy local. Stop LLM hallucinations when evaluating model metrics.

## Description
Language models are probabilistic text generators, not calculators. When asked to evaluate classification arrays to produce F1-Scores or Precision/Recall metrics, they frequently hallucinate decimals and fail edge cases. The Confusion Matrix Engine offloads this critical Data Science task to a deterministic, local JavaScript runtime. It accepts arrays of actual vs. predicted labels and instantly computes mathematically perfect True Positives, True Negatives, False Positives, False Negatives, and overall Accuracy.


## Available Tools
- **calculate_confusion_matrix**: Provide arrays of labels.

Calculates exact confusion matrix and accuracy from actual and predicted arrays


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Confusion Matrix Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here are my actual labels: ['cat','dog','cat']. And predictions: ['cat','cat','cat']. Calculate the exact accuracy and confusion matrix."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "I have 100 binary predictions (1s and 0s) and their actual outcomes. Can you generate the confusion matrix to find the False Positives?"

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Run these actual values and predicted values through the confusion matrix tool and tell me if the model is biased toward class A."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## Installation & Usage

To install and use the **Confusion Matrix Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confusion-matrix-engine](https://vinkius.com/mcp/confusion-matrix-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
