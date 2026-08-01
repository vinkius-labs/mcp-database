# Exact Levenshtein Distance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exact-levenshtein-distance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [text-processing](../categories/text-processing.md)

Compute precise edit distances and string similarity scores.

## Description
This MCP server provides high-precision algorithms for measuring the difference between two strings. It allows AI agents to calculate the exact Levenshtein edit distance, which counts insertions, deletions, and substitutions. Additionally, it supports Damerau-Levenshtein distance by accounting for transpositions of adjacent characters, and Jaro-Winkler similarity for a percentage-based matching score. This is essential for tasks involving spell checking, DNA sequence analysis, or fuzzy name matching.


## Available Tools (3)
- **damerau_levenshtein_distance**: Computes the Damerau-Levenshtein distance between two strings
- **jaro_winkler_similarity**: Computes the Jaro-Winkler similarity percentage between two strings
- **levenshtein_distance**: Computes the exact Levenshtein edit distance between two strings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exact Levenshtein Distance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Levenshtein distance between 'kitten' and 'sitting'?"

**🤖 AI Agent:**
> The Levenshtein distance between 'kitten' and 'sitting' is 3.

---

**👤 You:**
> "Calculate the Jaro-Winkler similarity for 'martha' and 'marhta'."

**🤖 AI Agent:**
> The Jaro-Winkler similarity score is approximately 100%.

---

**👤 You:**
> "Check the Damerau-Levenshtein distance for 'ca' and 'abc'."

**🤖 AI Agent:**
> The Damerau-Levenshtein distance is 2.


## ❓ FAQ

**Q: What is the difference between Levenshtein and Damerau-Levenshtein?**
Standard Levenshtein distance only considers insertions, deletions, and substitutions. `damerau_levenshtein_distance` also accounts for transpositions (swapping two adjacent characters) as a single edit.

**Q: Can I use this for fuzzy name matching?**
Yes, by using `jaro_winkler_similarity`, you can get a percentage score that is particularly effective for comparing names with small typographical errors.

**Q: Does it support large strings?**
The algorithms use dynamic programming matrices, making them highly accurate for any string length that fits within the agent's memory limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exact-levenshtein-distance-calculator](https://vinkius.com/mcp/exact-levenshtein-distance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exact Levenshtein Distance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exact-levenshtein-distance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exact Levenshtein Distance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exact-levenshtein-distance-calculator": {
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
