# String Metrics Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/string-metrics-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Bypass LLM tokenization blindness. Get exact character counts, word counts, and specific string occurrences deterministically.

## Description
LLMs suffer from absolute tokenization blindness. If you ask an AI "How many times does the letter R appear in the word Strawberry?", it frequently fails because it does not see letters—it sees tokens. This engine enforces deterministic character string auditing.

### The Superpowers

- **Token Blindness Bypass:** Instantly count the exact number of characters, spaces, and words in any text block using pure Node.js string mathematics.
- **Specific Substring Audits:** Ask the AI to verify exactly how many times a specific tag, word, or character appears in a generated document. The engine provides an irrefutable count.
- **SEO & Constraints:** Perfect for ensuring AI-generated SEO titles, meta descriptions, or ad copies stay strictly within character limits without hallucinating length.


## Available Tools
- **analyze_string_metrics**: Pass both strings and receive Levenshtein distance, Jaccard index, and other similarity scores for deduplication or fuzzy matching.

Deterministically calculates text metrics including exact character count, word count, and specific character occurrences to bypass LLM tokenization blindness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **String Metrics Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this blog text and calculate exactly how many times the substring 'Stripe' appears."

**🤖 AI Agent:**
> ✅ **String Metrics Analyzed:** The exact occurrence count for 'Stripe' is 14.

---

**👤 You:**
> "Count the absolute character length of this SEO description, including whitespaces."

**🤖 AI Agent:**
> ✅ **Length:** The string has exactly 168 characters natively measured in V8.

---

**👤 You:**
> "Does this meta title exceed the recommended 60 character threshold?"

**🤖 AI Agent:**
> ✅ **Evaluation:** Yes. The native count is 72, which exceeds the 60-character limit.


## ❓ FAQ

**Q: Why not just ask the LLM to count?**
Because LLMs process text in chunks called 'tokens', not individual characters.

**Q: Does it count whitespaces?**
Yes, it provides an exact Javascript string length.

**Q: Can it find how many times a word appears?**
Yes, substring occurrence counting is fully supported.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/string-metrics-analyzer](https://vinkius.com/mcp/string-metrics-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **String Metrics Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `string-metrics-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **String Metrics Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "string-metrics-analyzer": {
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
