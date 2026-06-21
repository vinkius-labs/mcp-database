# Language Detector Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/language-detector-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Detect the language of any text local using exact n-gram analysis. Supports 400+ languages. When AI guesses wrong on short or mixed text, this engine proves it.

## Description
Your customer support agent receives a ticket: 'O produto não chegou'. The AI routes it to the Spanish queue. The agent wastes time, the customer gets angry, SLA drops. Why? Because the AI 'guessed' the language probabilistically instead of calculating it.

This MCP uses `franc` (200K+ weekly downloads, inspired by Google's CLD2) to perform deterministic N-gram language detection. It returns exact ISO 639-3 codes for over 400 languages, and properly returns 'undefined' if a text is too ambiguous rather than hallucinating.

### The Superpowers

- **400+ Languages:** From English (eng) and Portuguese (por) to Esperanto (epo) and Zulu (zul).
- **Exact N-gram Math:** Analyzes text strictly by character frequencies, not LLM probability.
- **Whitelist/Blacklist:** Know the text must be either Spanish or Portuguese? Pass `only: ['spa', 'por']` to force a strict evaluation.
- **Confidence Scores:** Use the `all` flag to get an array of all matches with their exact probability scores.


## Available Tools
- **detect_language**: Provide as much text as possible for higher accuracy.

Detect the language of any text using n-gram analysis. Supports 400+ languages. Returns ISO 639-3 codes (e.g., "por", "eng", "spa")


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Language Detector Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Detect the language of this support ticket: 'Não consigo acessar minha conta desde ontem'."

**🤖 AI Agent:**
> Detected Language: 'por' (Portuguese). 100% confidence.

---

**👤 You:**
> "We only support English and Spanish. Detect the language of 'Hola como estas' using the whitelist."

**🤖 AI Agent:**
> Detected Language: 'spa' (Spanish) from the allowed list ['eng', 'spa'].

---

**👤 You:**
> "Get the top 3 language probabilities for this ambiguous name: 'Alejandro'."

**🤖 AI Agent:**
> Top Candidates: 1. spa (Spanish): 100% | 2. glg (Galician): 82% | 3. cat (Catalan): 64%


## ❓ FAQ

**Q: Why is this better than asking Claude to detect the language?**
LLMs often hallucinate languages for short strings or names. They also struggle to provide standardized ISO codes reliably. This engine uses mathematical N-gram analysis (the same technique behind Google Search language detection) to deterministically map text to one of 400+ ISO 639-3 codes.

**Q: What does it mean if it returns 'und'?**
'und' stands for Undefined. It means the text is too short, mostly numbers, or too ambiguous to confidently map to a single language. This is a feature — it prevents your routing logic from making false assumptions.

**Q: Can I force it to choose between specific languages?**
Yes. Pass an array of ISO 639-3 codes to the 'only' parameter (e.g., ['eng', 'por', 'spa']). The engine will only calculate probabilities within that subset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/language-detector-engine](https://vinkius.com/mcp/language-detector-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Language Detector Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `language-detector-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Language Detector Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "language-detector-engine": {
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
