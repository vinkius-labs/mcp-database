# AI Token Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-token-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Give AI Agents self-awareness of context limits. Count exact OpenAI/Claude tokens local to prevent fatal API truncation errors.

## Description
When a RAG Agent fetches 10 documents to summarize, it blindly sends them to the LLM API. If the payload exceeds the context window (e.g., 128k tokens), the API crashes, destroying the pipeline. LLMs cannot count their own tokens before sending a prompt. This MCP solves that perfectly.

### The Superpowers

- **Token Math:** Uses the exact `cl100k_base` encoding algorithm local to tell the Agent exactly how many tokens a payload contains.
- **Self-Aware Agents:** Allows Agents to do math and chunk their own massive datasets safely before hitting external API limits.


## Available Tools (1)
- **count_tokens**: Pass the raw text and receive the exact token count. Use the result to decide whether to chunk, summarize, or send directly.

Counts exact LLM tokens (cl100k_base) offline. Prevents RAG agents from exceeding context windows and crashing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Token Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me how many tokens are in this huge block of JSON data."

**🤖 AI Agent:**
> Token Count Result: There are 8540 tokens.

---

**👤 You:**
> "Count the tokens in this article so I know if I can fit it into my next prompt."

**🤖 AI Agent:**
> Token Count Result: The article has 2300 tokens.

---

**👤 You:**
> "I need the exact token count for this transcript snippet."

**🤖 AI Agent:**
> Token Count Result: Successfully counted.


## ❓ FAQ

**Q: What tokenizer algorithm is used?**
It uses the `cl100k_base` encoding, which is the exact algorithm used by GPT-3.5, GPT-4, and most Claude models.

**Q: Does it send my text to OpenAI?**
No. The calculation happens 100% local within the Edge engine using mathematical mapping.

**Q: Is it safe for large texts?**
Yes, it evaluates the exact token structure rapidly. But keep in mind standard Edge memory limits (under 10MB per payload).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-token-counter](https://vinkius.com/mcp/ai-token-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Token Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-token-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Token Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-token-counter": {
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
