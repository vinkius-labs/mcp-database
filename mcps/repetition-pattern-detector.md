# Repetition Pattern Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/repetition-pattern-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Detects redundant linguistic patterns and calculates text compression metrics.

## Description
This MCP server provides deterministic tools to identify recurring sequences of words within any text. By analyzing 3-gram phrases, it identifies structural redundancy and provides actionable metrics like repetition ratios and theoretical compression gains. Use `analyze_text_repetition` for a deep dive into redundancy, `get_repetition_summary` for a high-level overview, or `check_repetition_threshold` to verify if a text exceeds specific redundancy limits.


## Available Tools (3)
- **analyze_text_repetition**: Identifies repeating three-word sequences and calculates all redundancy and compression metrics
- **check_repetition_threshold**: Answers if the text exceeds a specific redundancy limit
- **get_repetition_summary**: Provides a high-level overview of text redundancy without the granular token counts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repetition Pattern Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for repetitions: 'The quick brown fox jumps over the lazy dog. The quick brown fox jumps over the lazy dog.'"

**🤖 AI Agent:**
> phraseCount: 10, repeatedPhrasesCount: 1, repetitionRatio: 0.1, tokensInRepetitions: 3, tokensSavedIfDeduped: 3, compressionRatio: 0.15

---

**👤 You:**
> "Give me a quick summary of the redundancy in: 'Redundancy is bad. Redundancy is bad. Redundancy is bad.'"

**🤖 AI Agent:**
> phraseCount: 3, repeatedPhrasesCount: 1, repetitionRatio: 0.33

---

**👤 You:**
> "Is the repetition ratio of 'Hello world hello world' above 0.2?"

**🤖 AI Agent:**
> isAboveThreshold: true, repetitionRatio: 0.33


## ❓ FAQ

**Q: What constitutes a repeated phrase?**
A phrase is defined as a sequence of exactly three consecutive words that appears two or more times in the text.

**Q: How is the compression ratio calculated?**
The compression ratio represents the theoretical percentage of the total word count that can be saved if all redundant repetitions are removed.

**Q: Can I check if my text is too repetitive?**
Yes, you can use the `check_repetition_threshold` tool to see if the repetition ratio exceeds a specific limit you define.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/repetition-pattern-detector](https://vinkius.com/ai-agent-connect/repetition-pattern-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repetition Pattern Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repetition-pattern-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repetition Pattern Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repetition-pattern-detector": {
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
