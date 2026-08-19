# Agent Semantic Deduplication Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-semantic-deduplication-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-agents](../categories/ai-agents.md)

A deterministic tool for calculating semantic similarity and deduplicating multi-agent outputs.

## Description
This MCP server provides a suite of tools to analyze and reduce redundancy in multi-agent systems. It uses cosine similarity to map relationships between agent outputs. Use `calculate_similarity_matrix` to generate a full map of semantic relationships, `identify_duplicate_clusters` to group similar outputs using single-linkage clustering, and `execute_deduplication` to apply strategies like `keep_first`, `keep_highest_confidence`, or `merge`. It is designed to help developers measure information loss and deduplication ratios in complex agentic workflows.


## Available Tools (3)
- **calculate_similarity_matrix**: Generates a complete map of semantic relationships between all provided agent outputs
- **execute_deduplication**: Applies a specific strategy to reduce the set of outputs to a unique set
- **identify_duplicate_clusters**: Groups redundant outputs into distinct semantic clusters based on a user-defined threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Semantic Deduplication Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the similarity matrix for these three agent outputs."

**🤖 AI Agent:**
> The similarity matrix has been generated. The similarity between output 1 and 2 is 0.98, indicating an exact duplicate.

---

**👤 You:**
> "Group these outputs into clusters with a threshold of 0.9."

**🤖 AI Agent:**
> Two clusters were identified: Cluster 1 contains agent IDs [A, B] and Cluster 2 contains [C].

---

**👤 You:**
> "Run deduplication using the keep_highest_confidence strategy."

**🤖 AI Agent:**
> Deduplication complete. The highest confidence output was selected for each cluster, resulting in a deduplication ratio of 0.75.


## ❓ FAQ

**Q: How do I find similar agent outputs?**
You can use the `calculate_similarity_matrix` tool to generate a matrix of cosine similarity scores between all provided agent outputs.

**Q: What is the difference between near-duplicates and exact duplicates?**
Near-duplicates have a similarity between 0.85 and 0.95, while exact duplicates have a similarity greater than 0.95.

**Q: Can I choose how duplicates are handled?**
Yes, the `execute_deduplication` tool allows you to choose between `keep_first`, `keep_highest_confidence`, or `merge` strategies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-semantic-deduplication-engine](https://vinkius.com/ai-agent-connect/agent-semantic-deduplication-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Semantic Deduplication Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-semantic-deduplication-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Semantic Deduplication Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-semantic-deduplication-engine": {
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
