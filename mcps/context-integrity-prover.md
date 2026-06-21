# Count Words for Agents MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/context-integrity-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Text analysis tool that counts words, characters, sentences, and paragraphs. Validates maximum length constraints so AI agents can generate text that strictly respects exact limits.

## Description
**Goal:** Provide exact text measurement to prevent agent hallucinations regarding length limits.

**Problem:** LLMs cannot natively count characters or words accurately. When given constraints like 'write a 280-character tweet' or 'summarize in under 500 words', agents often fail or hallucinate the counts. This breaks downstream automation workflows.

**Mechanism:** This MCP equips agents with deterministic validation tools. It calculates exact metrics for words, characters (with/without spaces), sentences, and paragraphs. Furthermore, passing the `max` parameter enables server-side threshold validation, instantly returning boolean `pass` metrics and remaining capacity.

**Advantage:** Agents can self-correct *before* outputting final responses. By validating their drafts against hard constraints, you guarantee compliance for SEO descriptions, social media APIs, and strict formatting guidelines.


## Available Tools (1)
- **text**: Use this strictly to measure character limits or string lengths without assuming any specific platform constraints.

Measures the exact character length of a text string, with or without spaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Count Words for Agents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you help me write an essay on climate change? It needs to be exactly between 400 and 500 words."

**🤖 AI Agent:**
> Here is your essay on climate change. I have verified its length: it is exactly 450 words, comfortably within your 400-500 word limit.

---

**👤 You:**
> "I need to post this update on Twitter/X, but I'm not sure if it fits. Can you check?"

**🤖 AI Agent:**
> Your text contains 250 characters (including spaces). This is within the 280-character limit, so you are good to post it on Twitter/X!

---

**👤 You:**
> "Write an introductory paragraph for my new blog. It must be exactly 3 sentences long."

**🤖 AI Agent:**
> Here is your introduction. I've structured it to be concise and impactful, and verified that it contains exactly 3 sentences as requested.

---

**👤 You:**
> "How long would it take the average person to read my 8-page newsletter draft?"

**🤖 AI Agent:**
> Based on an average reading speed of 200 words per minute, your newsletter draft of 3,150 words will take approximately 15 minutes and 45 seconds to read.


## ❓ FAQ

**Q: Can it count characters with and without spaces?**
Yes, the character counting tool provides an `includeSpaces` boolean option to include or exclude spaces.

**Q: How does limit validation work for agents?**
Agents pass an optional 'max' parameter. The server checks the count against the limit and returns a 'pass' true/false status, along with the percentage filled and characters/words remaining.

**Q: Can it calculate the reading time of an article?**
Yes, the estimate_reading_time tool calculates the duration based on a configurable words-per-minute baseline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context-integrity-prover](https://vinkius.com/mcp/context-integrity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Count Words for Agents** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `context-integrity-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Count Words for Agents** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "context-integrity-prover": {
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
