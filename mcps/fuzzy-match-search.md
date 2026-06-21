# Fuzzy Match Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fuzzy-match-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Perform lightning-fast fuzzy string matching across large datasets. Find the closest matches instantly using Levenshtein distance.

## Description
Asking an LLM to find the closest match to a misspelled name in an array of 5,000 customers consumes thousands of expensive tokens and takes seconds to process. This MCP brings ultra-fast `fuzzysort` algorithms to the edge, scoring and sorting targets instantly without eating your token budget.

### The Superpowers

- **Zero Token Waste:** Offload array searching from the LLM to the native V8 runtime.
- **Typo Tolerance:** Easily finds 'Jonnathon' when the target array contains 'Jonathan'. Includes exact match highlighting.


## Available Tools
- **fuzzy_match**: Pass a query and a JSON array of target strings. The engine uses fuzzy algorithms to find and rank the closest matches by similarity score.

Performs lightning-fast fuzzy string matching (Levenshtein-like) across an array of targets to find the closest matches to a query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fuzzy Match Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the closest match for 'appl' in this array of 50 fruit names."

**🤖 AI Agent:**
> ✅ **Matches Found:**
1. Target: `Apple`, Score: `-15`
2. Target: `Pineapple`, Score: `-40`

---

**👤 You:**
> "I need the top 3 matches for 'Jonathon' from my list of 10,000 customers."

**🤖 AI Agent:**
> ✅ **Matched:** The engine processed 10k items instantly. Best match is `Jonathan Meyers`.

---

**👤 You:**
> "Fuzzy search 'chk' against this array of bash commands."

**🤖 AI Agent:**
> ✅ **Result:** Matches `<b>ch</b>ec<b>k</b>out` with a high score.


## ❓ FAQ

**Q: How fast is it?**
It uses fuzzysort, which can process 100k strings in a few milliseconds.

**Q: Does it return a score?**
Yes, it returns a similarity score where numbers closer to 0 indicate a better match.

**Q: Does it highlight the match?**
Yes, it wraps the matched characters in HTML bold tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fuzzy-match-search](https://vinkius.com/mcp/fuzzy-match-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fuzzy Match Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fuzzy-match-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fuzzy Match Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fuzzy-match-search": {
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
