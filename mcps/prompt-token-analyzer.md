# Prompt Token Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/prompt-token-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministic token breakdown and budget analysis for prompt engineering.

## Description
This MCP server provides precise tools for managing token budgets in LLM workflows. It uses a deterministic 4-character-per-token ratio to calculate consumption across different prompt segments. Use `analyze_prompt_sections` for a detailed breakdown of tokens and budget adherence, `get_section_stats` for high-level summaries, or `find_outlier_sections` to identify bloated or empty sections. It helps developers optimize context windows and control costs effectively.


## Available Tools (3)
- **find_outlier_sections**: Identifies sections that are significantly larger or smaller than the average section size
- **analyze_prompt_sections**: Performs a full breakdown of a prompt's token consumption and budget adherence
- **get_section_stats**: Provides high-level summary statistics about the prompt's composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prompt Token Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these prompt sections: 'System: You are a helpful assistant' (35 chars) and 'User: Hello' (11 chars) with a budget of 20 tokens."

**🤖 AI Agent:**
> The total token count is 11.5 tokens. The budget remaining is 8.5 tokens. The largest section is 'System: You are a helpful assistant'.

---

**👤 You:**
> "Give me a summary of the token usage for these sections: 'Instruction' (12 chars) and 'Data' (100 chars) with a budget of 50 tokens."

**🤖 AI Agent:**
> Total tokens: 28. Budget remaining: 22. The system is within budget.

---

**👤 You:**
> "Find outliers in these sections: 'A' (1 char), 'B' (1 char), 'C' (1 char), and 'D' (100 chars)."

**🤖 AI Agent:**
> The large outlier is 'D'.


## ❓ FAQ

**Q: How is the token count calculated?**
The server uses a deterministic proxy where the token count is the total number of characters in a section divided by four.

**Q: Can I identify which parts of my prompt are too large?**
Yes, you can use the `find_outlier_sections` tool to identify sections that are significantly larger or smaller than the average size.

**Q: What happens if I exceed my token budget?**
The `analyze_prompt_sections` tool will return a negative budget remaining value and set the budget overrun flag to true.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/prompt-token-analyzer](https://vinkius.com/ai-agent-connect/prompt-token-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prompt Token Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prompt-token-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prompt Token Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prompt-token-analyzer": {
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
