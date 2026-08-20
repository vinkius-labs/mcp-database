# Multi-Language Token Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/multi-language-token-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze text composition and estimate token counts across multiple languages.

## Description
This MCP server provides deterministic linguistic analysis for mixed-language text. It uses character-level Unicode classification to identify English, Chinese, Japanese, Korean, Cyrillic, and Arabic content. Use `estimate_text_composition` to get a detailed breakdown of character counts, token estimates, and linguistic dominance, or `get_language_ratios` to view the fixed tokenization multipliers used for each language.


## Available Tools (3)
- **estimate_text_composition**: Analyzes a text string to provide a granular breakdown of character counts, token estimates, and linguistic dominance
- **get_language_ratios**: Retrieves the current deterministic token-to-character ratios used by the system
- **validate_unicode_range**: Verifies if a specific character belongs to one of the supported linguistic ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Language Token Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the composition of this text: 'Hello 世界'"

**🤖 AI Agent:**
> { "language_breakdown": [ { "language": "english", "chars": 5, "tokens": 20.0 }, { "language": "chinese", "chars": 2, "tokens": 3.0 } ], "total_tokens": 23.0, "dominant_language": "english", "language_mix_ratio": 0.714 }

---

**👤 You:**
> "What are the tokenization ratios used by this tool?"

**🤖 AI Agent:**
> { "ratios": { "english": 4.0, "chinese": 1.5, "japanese": 1.4, "korean": 1.8, "cyrillic": 2.8, "arabic": 2.5 } }

---

**👤 You:**
> "Is the character 'あ' supported?"

**🤖 AI Agent:**
> { "language": "japanese", "isValid": true }


## ❓ FAQ

**Q: How are tokens calculated?**
Tokens are estimated by multiplying the character count of each language by a specific deterministic ratio (e.g., 4.0 for English, 1.5 for Chinese).

**Q: Which languages are supported?**
The tool supports English, Chinese, Japanese, Korean, Cyrillic, and Arabic based on specific Unicode ranges.

**Q: Can I check specific character ranges?**
Yes, you can use `validate_unicode_range` to verify if a specific character belongs to a supported linguistic category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/multi-language-token-estimator](https://vinkius.com/ai-agent-connect/multi-language-token-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Language Token Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-language-token-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Language Token Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-language-token-estimator": {
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
