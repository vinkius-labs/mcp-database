# Token Count Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/token-count-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministic LLM token estimation using character-based heuristics.

## Description
This MCP server provides precise, deterministic estimation of LLM input sizes. By using model-specific linguistic ratios and structural density analysis, it calculates token counts for various architectures including GPT-4, Claude, Llama, and Gemma. Use `estimate_token_usage` to get a full breakdown of words, punctuation, and whitespace, or `analyze_text_complexity` to detect code and URL density. It also provides a confidence interval and warns when you are approaching the context window limit.


## Available Tools (3)
- **analyze_text_complexity**: Evaluates the structural characteristics of the text to prepare for specialized density calculations
- **estimate_token_usage**: Provides a comprehensive breakdown of the estimated token count and remaining capacity for a given input
- **get_model_ratios**: Retrieves the hardcoded character-to-token ratios for the specific model and language requested


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Token Count Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the token usage for this text: 'Hello, world!' using gpt-4 in english with a 4096 context window."

**🤖 AI Agent:**
> The estimated token count is 3 tokens, with 4093 tokens remaining in the context window.

---

**👤 You:**
> "Analyze the complexity of this code snippet: 'def add(a, b): return a + b'"

**🤖 AI Agent:**
> The text is identified as code with 1 detected numeric sequence and 0 URLs.

---

**👤 You:**
> "What is the character-to-token ratio for Claude in Chinese?"

**🤖 AI Agent:**
> The character-to-token ratio for Claude in Chinese is 1.2.


## ❓ FAQ

**Q: How accurate are these token estimates?**
The estimates use deterministic character-based heuristics. For English, we provide a ±10% confidence interval, while mixed languages use a ±15% interval.

**Q: Which models are supported?**
The server supports GPT-4, Claude, Llama, and Gemma through specific character-to-token ratios.

**Q: Can I detect if my text is too long for the model?**
Yes, the `estimate_token_usage` tool includes an `isOverCapacityWarning` flag that triggers when you exceed 90% of the specified context window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/token-count-estimator](https://vinkius.com/ai-agent-connect/token-count-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Token Count Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `token-count-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Token Count Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "token-count-estimator": {
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
