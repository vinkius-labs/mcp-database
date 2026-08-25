# Markdown Code Block Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/markdown-code-block-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [parsing](../categories/parsing.md)

Extracts exact code blocks from LLM markdown responses.

## Description
This MCP server provides precise extraction of code segments from LLM-generated Markdown. It uses a strict character-level state machine to identify fenced blocks, indented blocks, and inline code, ensuring high fidelity for downstream processing. Use `extract_code_blocks` to retrieve all segments, `validate_block_integrity` to verify structural accuracy, and `get_block_metadata` to inspect specific block properties.


## Available Tools (3)
- **get_block_metadata**: Provides context about the nature of a specific extracted block
- **validate_block_integrity**: Checks if the extracted blocks actually match the original structural intent of the Markdown
- **extract_code_blocks**: Performs the primary extraction of all code segments within a provided Markdown string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Code Block Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the code from this markdown: ```python
print('hello')
```"

**🤖 AI Agent:**
> print('hello')

---

**👤 You:**
> "What is the language of the first code block in this text?"

**🤖 AI Agent:**
> The language is python.

---

**👤 You:**
> "Check if the extracted blocks are valid for this content: # Title
    print(1)"

**🤖 AI Agent:**
> true


## ❓ FAQ

**Q: What types of code blocks can be extracted?**
The server extracts fenced blocks (triple backticks), indented blocks (4 spaces or tab), and inline code (single backticks).

**Q: How do I verify if the extraction was successful?**
You can use the `validate_block_integrity` tool to ensure the extracted segments perfectly reconstruct the original Markdown structure.

**Q: Can I see the language of a specific block?**
Yes, use `get_block_metadata` with the specific block index to retrieve the language identifier and block type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/markdown-code-block-extractor](https://vinkius.com/ai-agent-connect/markdown-code-block-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markdown Code Block Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `markdown-code-block-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markdown Code Block Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markdown-code-block-extractor": {
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
