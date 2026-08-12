# agent-output-deduplicator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agent-output-deduplicator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Detects and removes redundant outputs from multi-agent workflows using Jaccard similarity and n-gram overlap.

## Description
This MCP server provides specialized tools to identify and prune overlapping information produced by multiple autonomous agents. It uses mathematical similarity measures like Jaccard word-set similarity and n-gram overlap (n=2 or n=3) to flag redundant content. When duplicates are found, the server can automatically select a canonical output based on agent priority or execution order. Key tools include `get_similarity_score` for direct comparisons, `identify_duplicates` for scanning entire collections, and `resolve_canonical_selection` for picking the best surviving output.


## Available Tools (3)
- **get_similarity_score**: Calculates the mathematical similarity between two specific text strings using n-grams
- **identify_duplicates**: Scans a collection of agent outputs to find clusters of redundant information
- **resolve_canonical_selection**: Determines which specific output should be kept when multiple similar outputs are identified


## 💬 Prompt Examples

Here are some examples of how you can interact with the **agent-output-deduplicator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two agent outputs for redundancy."

**🤖 AI Agent:**
> The similarity score between the two outputs is 0.92, meaning they are highly redundant.

---

**👤 You:**
> "Find all duplicate clusters in this list of agent results."

**🤖 AI Agent:**
> I found 2 duplicate clusters. The first cluster contains 3 redundant outputs, and the second contains 2.

---

**👤 You:**
> "Which output should I keep from this group of similar results?"

**🤖 AI Agent:**
> The canonical output is ID 'out_001' because it was produced by the highest priority agent.


## ❓ FAQ

**Q: How does the similarity calculation work?**
The server uses Jaccard similarity and n-gram overlap. It calculates the intersection of word sequences divided by the union of those sequences to determine how much two texts overlap.

**Q: How is the canonical output chosen?**
The `resolve_canonical_selection` logic prioritizes the output from the agent with the highest numerical priority. If priorities are tied, the output that appeared first in the sequence is selected.

**Q: Can I configure the similarity threshold?**
Yes, when using `identify_duplicates`, you can provide a custom threshold value between 0 and 1 to define what constitutes a duplicate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agent-output-deduplicator](https://vinkius.com/mcp/agent-output-deduplicator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **agent-output-deduplicator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-output-deduplicator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **agent-output-deduplicator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-output-deduplicator": {
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
