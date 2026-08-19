# Code Block Token Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/code-block-token-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate token density and code-to-text ratios in documents.

## Description
This MCP server provides deterministic analysis of text containing code blocks. It calculates token counts by applying specific density heuristics: code tokens are estimated at 3 characters per token, while non-code text is estimated at 4 characters per token. Use `analyze_text_density` to get a full breakdown of code blocks, character counts, and token ratios, or `get_token_metrics_summary` for a high-level overview of token distribution. It also includes `validate_code_block_format` to ensure text contains extractable triple-backtick blocks.


## Available Tools (3)
- **validate_code_block_format**: 
- **analyze_text_density**: 
- **get_token_metrics_summary**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Code Block Token Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the token density of this text: 'Here is some code: ```const x = 10;```'"

**🤖 AI Agent:**
> code_block_count: 1, total_code_chars: 14, code_tokens: 4, non_code_tokens: 4, total_tokens: 8, code_ratio: 0.5, optimization_suggested: false

---

**👤 You:**
> "Give me a summary of the token metrics for: '```print(hello)```'"

**🤖 AI Agent:**
> total_tokens: 4, code_ratio: 1.0, is_code_heavy: true

---

**👤 You:**
> "Does this text contain valid code blocks: 'Just some plain text here.'"

**🤖 AI Agent:**
> has_code_blocks: false, block_count: 0


## ❓ FAQ

**Q: How are tokens calculated?**
Code tokens are calculated by dividing code characters by 3, and non-code tokens by 4.

**Q: What is the purpose of the optimization suggestion?**
If the code ratio exceeds 0.5, the tool suggests summarizing or extracting code to optimize context window usage.

**Q: Can I check if my text has valid code blocks?**
Yes, you can use the `validate_code_block_format` tool to verify if triple-backtick blocks are present.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/code-block-token-analyzer](https://vinkius.com/ai-agent-connect/code-block-token-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Code Block Token Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `code-block-token-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Code Block Token Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "code-block-token-analyzer": {
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
