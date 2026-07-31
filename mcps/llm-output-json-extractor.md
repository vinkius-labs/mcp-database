# LLM Output JSON Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-output-json-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Isolates valid JSON objects from mixed markdown/text LLM outputs using deterministic bracket-matching.

## Description
The LLM Output JSON Extractor is a precision utility designed to solve the problem of 'chatty' AI responses. When LLMs wrap useful data in backticks, introduce conversational filler, or start with introductory text like 'Here is your JSON:', this MCP server provides a deterministic way to extract the payload. Using a robust bracket-matching algorithm, it identifies the first completed structure that passes structural validation. It is ideal for developers building automated pipelines where reliable JSON extraction from unstructured text is critical. Use `extract_json` to pull payloads, `validate_structure` to verify syntax, and `get_extraction_metadata` to analyze noise reduction.


## Available Tools (3)
- **extract_json**: Extracts the first valid JSON object from a raw string
- **get_extraction_metadata**: Provides metrics on the extraction process
- **validate_structure**: parse() without errors.

Validates if a string is syntactically correct JSON


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM Output JSON Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the JSON from this text: 'Sure! Here is your data: ```json {"status": "success"} ``` Hope this helps!'"

**🤖 AI Agent:**
> {"status": "success"}

---

**👤 You:**
> "Is this string valid JSON: '{"name": "test",}'"

**🤖 AI Agent:**
> false

---

**👤 You:**
> "How much noise was removed from this input?"

**🤖 AI Agent:**
> The extraction process identified the JSON payload and calculated the reduction ratio based on the discarded text.


## ❓ FAQ

**Q: How does the extractor handle multiple JSON objects in one string?**
The extractor scans from left to right and stops at the very first completed structure that passes structural validation.

**Q: Can I use this to check if a string is valid JSON?**
Yes, you can use the `validate_structure` tool to confirm if a specific segment of text is syntactically correct and parsable.

**Q: What happens if the braces are unbalanced?**
If the parser detects unbalanced braces, it will mark `isValid` as false and return an empty string for the extracted content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-output-json-extractor](https://vinkius.com/mcp/llm-output-json-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM Output JSON Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-output-json-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM Output JSON Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-output-json-extractor": {
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
