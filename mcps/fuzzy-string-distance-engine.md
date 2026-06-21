# Fuzzy String Distance Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fuzzy-string-distance-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate exact Levenshtein, Jaro-Winkler, and Dice distances for fuzzy text matching natively local.

## Description
When deduplicating lists of names or correcting misspellings (e.g. 'John Smith' vs 'Jon Smyth'), semantic embeddings are overkill and LLM prompting is unpredictable. This engine provides the academic gold-standard string distances: Levenshtein (edit distance), Jaro-Winkler (prefix-heavy similarity), and Dice coefficient. Computed strictly in local JS, it gives agents a mathematical foundation for entity resolution.


## Available Tools
- **calculate_fuzzy_distance**: Calculates deterministic Levenshtein, Jaro-Winkler, and Dice string distances between two texts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fuzzy String Distance Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Jaro-Winkler distance between 'Vinkius' and 'Vinckius'. Is the similarity above 0.9?"

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "What is the exact Levenshtein edit distance between 'kitten' and 'sitting'?"

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Run the fuzzy distance engine on 'Jonathan Doe' and 'Jon Doe'. If Dice coefficient > 0.8, treat them as the same entity."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: When should I use Levenshtein?**
Levenshtein counts the absolute number of character edits (insertions, deletions, substitutions) required to match the strings. Great for simple spell-checks.

**Q: When is Jaro-Winkler better?**
Jaro-Winkler gives a score from 0 to 1 and heavily weights matching prefixes. It is the industry standard for matching personal names in databases.

**Q: Why not use embeddings?**
Embeddings match *meaning* (semantics). Fuzzy string distances match *characters* (lexical). If you want to match 'cat' to 'catt', string distance is better.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fuzzy-string-distance-engine](https://vinkius.com/mcp/fuzzy-string-distance-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fuzzy String Distance Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fuzzy-string-distance-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fuzzy String Distance Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fuzzy-string-distance-engine": {
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
