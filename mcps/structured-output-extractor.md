# Structured Output Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/structured-output-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Recover structured data from malformed LLM responses using deterministic regex.

## Description
When Large Language Models fail to follow strict JSON or Pydantic schemas due to conversational filler, this MCP server acts as a rescue engine. It uses deterministic regex patterns to find signal within the noise, treating user-provided field names as anchors. You can use `extract_structured_data` to pull specific fields, `validate_schema_integrity` to ensure your schema is valid, and `get_extraction_summary` to evaluate the reliability of the results. It is designed to bridge the gap between messy LLM text and the structured data your applications require.


## Available Tools (3)
- **extract_structured_data**: Performs the primary rescue extraction of fields from a block of text using a provided schema
- **validate_schema_integrity**: Checks if the provided schema definition is logically sound and follows naming conventions
- **get_extraction_summary**: Provides a high-level overview of a specific extraction attempt's success and reliability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Structured Output Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the name and age from this text: 'The user's name is Alice and she is 30 years old.' with schema {"name": "string", "age": "number"}"

**🤖 AI Agent:**
> {"name": "Alice", "age": 30}

---

**👤 You:**
> "Extract the status from: 'The task is completed: yes.' with schema {"status": "boolean"}"

**🤖 AI Agent:**
> true

---

**👤 You:**
> "Extract the items from: 'Shopping list: - apples, - milk, - bread' with schema {"items": "list"}"

**🤖 AI Agent:**
> ["apples", "milk", "bread"]


## ❓ FAQ

**Q: How does this tool extract data without using an LLM?**
The tool uses deterministic regex patterns to locate field names (anchors) and extract the subsequent values based on the expected type (string, number, boolean, or list).

**Q: What happens if the LLM response is completely unstructured?**
The `extract_structured_data` tool will attempt to find the requested fields. If the patterns do not match, the fields will be returned in the `missingFields` list with a low confidence score.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes. You can connect this MCP server to Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/structured-output-extractor](https://vinkius.com/mcp/structured-output-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Structured Output Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `structured-output-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Structured Output Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "structured-output-extractor": {
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
