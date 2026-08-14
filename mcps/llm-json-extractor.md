# LLM JSON Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-json-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Isolates valid JSON objects from messy LLM text outputs.

## Description
This MCP server provides specialized tools to extract structured JSON payloads from unstructured, conversational, or markdown-formatted Large Language Model (LLM) responses. It uses deterministic bracket-matching to identify the boundaries of the first valid JSON object or array, even when surrounded by conversational noise. Use `extract_first_json_payload` to find the payload, `verify_json_integrity` to check syntax, and `get_extraction_metadata` to retrieve character offsets and markdown wrapper information.


## Available Tools (3)
- **extract_first_json_payload**: Attempts to find and isolate the first valid JSON object or array within a raw string
- **get_extraction_metadata**: Calculates the location and length properties of a detected JSON payload
- **verify_json_integrity**: Validates if a specific substring is a syntactically correct JSON structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM JSON Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the JSON from this text: Here is your data: {"id": 123, "status": "ok"} hope this helps!"

**🤖 AI Agent:**
> {"id": 123, "status": "ok"}

---

**👤 You:**
> "Find the JSON in this markdown: ```json [1, 2, 3] ```"

**🤖 AI Agent:**
> [1, 2, 3]

---

**👤 You:**
> "Is this valid JSON: {"key": "value",}"

**🤖 AI Agent:**
> No, it is invalid due to a trailing comma.


## ❓ FAQ

**Q: How does the extraction work?**
The server uses a scan-based approach with a counter to track opening and closing braces and brackets, ensuring nested structures are fully captured.

**Q: Can it handle markdown code blocks?**
Yes, the `get_extraction_metadata` tool can specifically identify if the detected JSON is wrapped in markdown code blocks.

**Q: What happens if the JSON is invalid?**
The `verify_json_integrity` tool will return a failure status and a human-readable reason explaining why the syntax is incorrect.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-json-extractor](https://vinkius.com/mcp/llm-json-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM JSON Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-json-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM JSON Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-json-extractor": {
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
