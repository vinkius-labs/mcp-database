# Long-Tail Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/long-tail-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Identify recurring word sequences (n-grams) to discover potential long-tail keyword candidates within any text.

## Description
The Long-Tail Extractor is a specialized analysis engine designed to uncover hidden patterns in large bodies of text. By identifying contiguous blocks of words--specifically 3, 4, and 5-word sequences (n-grams)--it helps users discover high-potential long-tail keyword candidates for SEO and content strategy. The server provides three powerful tools: `extract_ngram_sequences` to scan text for recurring phrases, `filter_high_frequency_patterns` to isolate significant patterns based on a frequency threshold, and `calculate_pattern_density` to measure the prevalence of these sequences relative to the total word count. This tool automates the tedious process of manual text analysis, providing precise data on phrase frequency and position.


## Available Tools (3)
- **extract_ngram_sequences**: Returns phrases with their counts and positions.

Identify recurring sequences of words within a text
- **filter_high_frequency_patterns**: Filter N-grams by a minimum frequency threshold
- **calculate_pattern_density**: Calculate the density of N-grams within a text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Long-Tail Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all recurring 3-word sequences in this text: 'The quick brown fox jumps over the lazy dog. The quick brown fox is very fast.'"

**🤖 AI Agent:**
> Found 1 recurring sequence: 'the quick brown' (2 occurrences).

---

**👤 You:**
> "Filter these n-grams to only show those that appear at least 3 times: '[{"phrase": "apple pie", "count": 1}, {"phrase": "banana split", "count": 4}]'"

**🤖 AI Agent:**
> The following patterns met the threshold: 'banana split'.

---

**👤 You:**
> "Calculate the density for 'hello world' which appears 2 times in a text of 100 words."

**🤖 AI Agent:**
> The density score for 'hello world' is 0.02.


## ❓ FAQ

**Q: What are n-grams?**
N-grams are contiguous sequences of $n$ items from a given sample of text. In this tool, we focus on sequences of 3, 4, and 5 words.

**Q: How can I use `extract_ngram_sequences`?**
Provide the raw text you want to analyze via the `sourceText` parameter. You can also specify a minimum and maximum n-gram size.

**Q: What is the purpose of density calculation?**
The `calculate_pattern_density` tool calculates how often a phrase appears relative to the total word count, helping you distinguish significant patterns from isolated occurrences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/long-tail-extractor](https://vinkius.com/mcp/long-tail-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Long-Tail Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `long-tail-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Long-Tail Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "long-tail-extractor": {
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
