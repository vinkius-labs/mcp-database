# LLM JSON Repair Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-json-repair-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Fixes malformed, truncated, or dirty JSON strings produced by LLMs.

## Description
This MCP server provides deterministic, character-level repair for JSON strings that fail to meet RFC 8259 standards. It is designed to handle common LLM failures such as trailing commas, unquoted keys, single quotes, and structural truncation where braces or brackets are left unclosed. Using a state-machine approach, it ensures predictable results without hallucinating data. You can use `repair_json_string` to fix broken structures, `validate_json_integrity` to check for syntax violations, and `extract_json_from_text` to pull JSON out of conversational filler or markdown blocks.


## Available Tools (3)
- **extract_json_from_text**: 
- **repair_json_string**: 
- **validate_json_integrity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM JSON Repair Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fix this broken JSON: {"name": 'John', "age": 30,}"

**🤖 AI Agent:**
> {"name": "John", "age": 30}

---

**👤 You:**
> "Extract the JSON from this text: Here is the data: ```json {"id": 123} ``` Hope this helps!"

**🤖 AI Agent:**
> {"id": 123}

---

**👤 You:**
> "The LLM cut off here: {"items": [{"id": 1}, {"id": 2"

**🤖 AI Agent:**
> {"items": [{"id": 1}, {"id": 2}]}


## ❓ FAQ

**Q: How does this differ from using an LLM to fix JSON?**
Unlike probabilistic LLMs, this server uses a deterministic state machine. This means it only fixes structural issues like missing brackets or trailing commas without inventing or changing the actual data content.

**Q: Can I extract JSON from a long chat response?**
Yes, you can use the `extract_json_from_text` tool to locate and isolate the JSON object or array within a larger block of conversational text.

**Q: What happens if the JSON is truncated due to token limits?**
The `repair_json_string` tool tracks the nesting depth of all open braces and brackets and automatically appends the necessary closing characters to restore structural integrity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-json-repair-utility](https://vinkius.com/mcp/llm-json-repair-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM JSON Repair Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-json-repair-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM JSON Repair Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-json-repair-utility": {
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
