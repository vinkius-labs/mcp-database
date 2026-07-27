# Markdown Table to JSON Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-table-to-json-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Convert GitHub-flavored Markdown tables into structured JSON arrays of objects.

## Description
The Markdown Table to JSON Converter is a specialized utility designed for reliable data extraction from unstructured text. It allows AI agents to transform GitHub-flavored Markdown (GFM) tables into exact, deterministic JSON arrays of objects. By using tools like `convert_table_to_json`, `validate_table_structure`, and `extract_all_tables`, you can bridge the gap between visual markdown formatting and structured data processing. This ensures that even complex documents with multiple tables are parsed with high precision, maintaining column integrity and cell sanitization.


## Available Tools (3)
- **convert_table_to_json**: Convert a markdown table to a JSON array
- **extract_all_tables**: Extract all markdown tables from a document
- **validate_table**: Validate the structure of a markdown table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Table to JSON Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this table to JSON: | Name | Age |
|---|---|
| Alice | 30 |
| Bob | 25 |"

**🤖 AI Agent:**
> [{"Name": "Alice", "Age": "30"}, {"Name": "Bob", "Age": "25"}]

---

**👤 You:**
> "Is this markdown block a valid table?"

**🤖 AI Agent:**
> The validation check confirms the structure is correct and follows GFM standards.

---

**👤 You:**
> "Extract all tables from this text: 'Here is a table: | A | B |
|---|---|
| 1 | 2 |' and 'Another one: | C | D |
|---|---|
| 3 | 4 |'"

**🤖 AI Agent:**
> Two tables were found and processed into JSON arrays.


## ❓ FAQ

**Q: What kind of Markdown tables does this support?**
It supports GitHub-flavored Markdown (GFM) tables that use the pipe (|) delimiter and include a proper header separator row.

**Q: Can I extract multiple tables from a single document?**
Yes, you can use the `extract_all_tables` tool to scan an entire document and retrieve every identifiable table as a separate entry.

**Q: Does the converter clean up whitespace in cells?**
Yes, all extracted values are automatically trimmed of leading and trailing whitespace to ensure data integrity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-table-to-json-converter](https://vinkius.com/mcp/markdown-table-to-json-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markdown Table to JSON Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `markdown-table-to-json-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markdown Table to JSON Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markdown-table-to-json-converter": {
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
