# LLM Token Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-token-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate exact and estimated token counts for GPT-4, GPT-4o, Claude, and Llama models.

## Description
An essential utility for LLM developers to manage context windows. Use `token_count` to get precise token counts across multiple encodings like cl100k_base and o200k_base, or use `analyze_complexity` to evaluate text linguistic patterns. This MCP server helps you calculate chat template overhead and find optimal truncation points to prevent context overflow in models like GPT-4o and Claude.


## Available Tools (2)
- **analyze_complexity**: Analyze text complexity and punctuation diversity
- **token_count**: Calculate character, word, and estimated token counts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM Token Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many tokens are in the string 'Hello, world!' using o200k_base?"

**🤖 AI Agent:**
> The string 'Hello, world!' contains 3 tokens using the o200k_base encoding.

---

**👤 You:**
> "Analyze the complexity of this text: 'The quick brown fox jumps over the lazy dog.'"

**🤖 AI Agent:**
> The text has a complexity score of 1.2 and shows low punctuation diversity.

---

**👤 You:**
> "Calculate the overhead for a user message with content 'Hi' and role 'user'."

**🤖 AI Agent:**
> The total tokens for this message, including structural delimiters, is 5 tokens.


## ❓ FAQ

**Q: Which LLM tokenizers are supported?**
The server provides exact counts for `cl100k_base` (GPT-4) and `o200k_base` (GPT-4o), as well as approximations for Claude and SentencePiece-based models like Llama.

**Q: How does the tool handle chat message overhead?**
The `calculate_chat_overhead` logic accounts for the hidden structural tokens (like role indicators and delimiters) added by API templates to ensure your total token count is accurate.

**Q: Can I use this for text truncation?**
Yes, you can use the `find_truncation_point` tool to determine exactly where to trim your input text to stay within a specific token budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-token-counter](https://vinkius.com/mcp/llm-token-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM Token Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-token-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM Token Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-token-counter": {
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
