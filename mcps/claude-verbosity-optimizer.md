# Claude Verbosity Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claude-verbosity-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic engine to detect and compress verbose LLM outputs to preserve context window budget.

## Description
The Claude Verbosity Optimizer is a deterministic toolset designed to prevent context bloat in AI conversations. It identifies redundant reasoning, repetitive descriptions, and narrative filler using mathematical rules like Jaccard similarity. By using `compress_text`, users can automatically apply rules such as redundant sentence removal, file list collapsing, and code block sanitization to stay within strict token limits. It provides precise control over context management without the unpredictability of LLM-based summarization.


## Available Tools (3)
- **analyze_verbosity**: Assess the current state of a text block and determine how much waste exists relative to a specific budget
- **compress_text**: Execute deterministic reduction rules on a given text block to meet a token budget
- **get_optimization_report**: Provide a structured overview of the optimization effectiveness for auditing purposes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Verbosity Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this response for verbosity: 'I will now proceed to analyze the code. I am analyzing the code. The code is being analyzed by me.' with a budget of 50 tokens."

**🤖 AI Agent:**
> The `analyze_verbosity` tool indicates high redundancy due to the repetitive nature of the sentences.

---

**👤 You:**
> "Compress this text to 20 tokens: 'The user requested a file list. Modified file1.ts, modified file2.ts, modified file3.ts, modified file4.ts.'"

**🤖 AI Agent:**
> Modified 4 files in the project.

---

**👤 You:**
> "How can I see how much space I saved after compression?"

**🤖 AI Agent:**
> You can use the `get_optimization_report` tool to compare the original and optimized text and see the exact compression ratio.


## ❓ FAQ

**Q: How does this tool ensure compression is deterministic?**
Unlike LLM summarization, this tool uses mathematical rules like Jaccard similarity and structural patterns to remove text, ensuring the technical meaning remains unchanged.

**Q: What is the difference between `analyze_verbosity` and `compress_text`?**
The `analyze_verbosity` tool assesses the current redundancy and estimated savings, while `compress_text` actively applies the reduction rules to meet your specific token budget.

**Q: Can I use this to clean up long file lists in my chat history?**
Yes, the `compress_text` tool includes a file list collapse rule that replaces long lists of changed files with a concise summary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claude-verbosity-optimizer](https://vinkius.com/ai-agent-connect/claude-verbosity-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Verbosity Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-verbosity-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Verbosity Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-verbosity-optimizer": {
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
