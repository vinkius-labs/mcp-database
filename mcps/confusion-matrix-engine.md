# Confusion Matrix Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/confusion-matrix-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministically calculate True Positives, FP, Precision, Recall, F1-Score, and Accuracy local. Stop LLM hallucinations when evaluating model metrics.

## Description
Language models are probabilistic text generators, not calculators. When asked to evaluate classification arrays to produce F1-Scores or Precision/Recall metrics, they frequently hallucinate decimals and fail edge cases. The Confusion Matrix Engine offloads this critical Data Science task to a deterministic, local JavaScript runtime. It accepts arrays of actual vs. predicted labels and instantly computes mathematically perfect True Positives, True Negatives, False Positives, False Negatives, and overall Accuracy.


## Available Tools (1)
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


## ❓ FAQ

**Q: Why not let Claude/GPT calculate the accuracy?**
LLMs operate on tokens and probability distributions. If you give them 500 predictions, they might summarize or estimate the F1-score rather than calculating it exactly. This engine ensures 100% mathematical precision.

**Q: Does it support multi-class classification?**
Yes, the engine automatically detects unique labels from both arrays and constructs an N-by-N confusion matrix, handling both binary and multiclass evaluations flawlessly.

**Q: Is there a limit to the array size?**
The only limit is the standard Context Window limit for transmitting the JSON arrays. For arrays exceeding 100k items, consider chunking or local CSV aggregators.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confusion-matrix-engine](https://vinkius.com/mcp/confusion-matrix-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Confusion Matrix Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `confusion-matrix-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Confusion Matrix Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "confusion-matrix-engine": {
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
