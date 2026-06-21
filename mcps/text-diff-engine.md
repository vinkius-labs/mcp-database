# Text Diff Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/text-diff-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Exact character-by-character string comparison. Stop relying on LLM summaries and get absolute text diffs for code and contracts.

## Description
LLMs summarize differences rather than showing them exactly. This MCP uses the `diff` library to provide deterministic, line-by-line patch generation.

### The Superpowers

- **Exact Patches:** See exactly which characters or lines were added or removed.


## Available Tools
- **compare_texts**: Pass the original and modified versions and receive a structured diff with additions, deletions, and unchanged lines.

Performs an exact line-by-line diff comparison between two strings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Text Diff Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a unified diff between `v1-config.json` and `v2-config.json`."

**🤖 AI Agent:**
> ✅ **Diff Generated:**
```diff
-  "timeout": 30
+  "timeout": 60
```

---

**👤 You:**
> "Show me the word-level differences between these two legal contract paragraphs."

**🤖 AI Agent:**
> ✅ **Word Diff:** Detected 4 removed words and 2 added clauses accurately.

---

**👤 You:**
> "Compare the original HTML file with the minified version to ensure no attribute loss."

**🤖 AI Agent:**
> ✅ **Comparison Complete:** The files are structurally identical, differing only in 1,204 whitespace removals.


## ❓ FAQ

**Q: Can it diff code?**
Yes, it is excellent for comparing code files.

**Q: Does it output in standard patch format?**
Yes, it outputs unified diff formatting.

**Q: Can it diff large documents?**
Absolutely, it runs instantly on large text payloads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/text-diff-engine](https://vinkius.com/mcp/text-diff-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Text Diff Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `text-diff-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Text Diff Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "text-diff-engine": {
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
