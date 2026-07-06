# String Similarity Batch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/string-similarity-batch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

High-performance string similarity computations for batch processing of large text arrays using algorithms like Levenshtein and Jaro-Winkler.

## Description
This MCP server provides precise, matrix-based string comparison metrics that are computationally expensive for LLMs. Use `batch_rank_candidates` to rank an array of strings against a target using metrics like `levenshtein`, `jaro_winkler`, or `sorensen_dice`. Alternatively, use `compute_single_metric` for one-to-one comparisons between two specific strings. It handles strings up to 5000 characters and supports algorithms including Damerau-Levenshtein and Longest Common Subsequence (LCS).


## Available Tools (2)
- **batch_rank_candidates**: Rank candidates based on similarity to a target
- **compute_single_metric**: for example Levenshtein) between two strings.

Compute a string similarity metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **String Similarity Batch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these names by Jaro-Winkler similarity to 'John': ['Jon', 'Johnny', 'James']"

**🤖 AI Agent:**
> 1. Jon (0.85), 2. Johnny (0.78), 3. James (0.62)

---

**👤 You:**
> "What is the Levenshtein distance between 'kitten' and 'sitting'?"

**🤖 AI Agent:**
> The Levenshtein distance between 'kitten' and 'sitting' is 3.

---

**👤 You:**
> "Compare 'apple' and 'apply' using LCS."

**🤖 AI Agent:**
> The Longest Common Subsequence (LCS) length for 'apple' and 'apply' is 4.


## ❓ FAQ

**Q: Can I use this for large datasets?**
Yes, the `batch_rank_canditates` tool is designed to process arrays of candidates efficiently.

**Q: What is the maximum string length?**
Each individual string can be up to 5000 characters.

**Q: Does it support Jaro-Winkler?**
Yes, `jaro_winkler` is one of the supported metric types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/string-similarity-batch](https://vinkius.com/mcp/string-similarity-batch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **String Similarity Batch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `string-similarity-batch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **String Similarity Batch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "string-similarity-batch": {
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
