# Reasoning Step Word Count Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reasoning-step-word-count-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyze ReAct traces to audit reasoning verbosity and detect zero-shot behavior.

## Description
The Reasoning Step Word Count Analyzer MCP server provides a specialized auditing engine for evaluating the quality of ReAct (Reasoning, Acting) traces. By calculating exact word counts between 'Thought' and 'Action' phases, it determines reasoning verbosity ratios and identifies potential zero-shot patterns where thought blocks are too brief (< 10 words). This is essential for developers monitoring chain-of-thought performance in LLM agents.


## Available Tools (3)
- **calculate_verbosity_ratio**: Calculates the ratio of thought text to action text
- **detect_zero_shot_behavior**: Detects if the model exhibits zero-shot behavior based on thought word count
- **parse_react_trace**: Parses a React trace string to extract structured information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reasoning Step Word Count Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this ReAct trace: Thought: I need to find the weather. Action: search(weather in London)."

**🤖 AI Agent:**
> The parsed trace contains a thought phase and an action phase. The verbosity ratio is calculated based on the word counts of these segments.

---

**👤 You:**
> "Is this trace showing zero-shot behavior? Thought: Okay. Action: print(hello)"

**🤖 AI Agent:**
> Yes, the thought block contains only 1 word, which is below the 10-word threshold for complex reasoning.

---

**👤 You:**
> "Calculate the ratio for: Thought: I will check the stock price. Action: get_stock(AAPL)"

**🤖 AI Agent:**
> The verbosity ratio is 0.75, based on a thought count of 7 words and an action count of 9 words.


## ❓ FAQ

**Q: How does the analyzer detect zero-shot behavior?**
The `detect_zero_shot_behavior` tool analyzes the word count of a thought block. If the count is below the threshold, it flags the trace as likely zero-shot behavior.

**Q: Can I use this to compare different model traces?**
Yes. By using `calculate_verbosity_ratio`, you can quantitatively compare the reasoning depth of different models by examining their thought-to-action text ratios.

**Q: What input format is required for parsing?**
The `parse_react_trace` tool accepts a raw string containing the ReAct trace. It uses exact whitespace splitting to extract structured components.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reasoning-step-word-count-analyzer](https://vinkius.com/mcp/reasoning-step-word-count-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reasoning Step Word Count Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reasoning-step-word-count-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reasoning Step Word Count Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reasoning-step-word-count-analyzer": {
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
