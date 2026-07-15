# JSON Schema Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-schema-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [development](../categories/development.md)

Validate JSON documents and lint schemas for structural integrity.

## Description
The JSON Schema Validator MCP server provides high-precision validation of JSON documents against Draft-07 and 2020-12 specifications. Use `validate_json_document` to check if a document adheres to your schema, identifying exact paths to errors. The `lint_json_schema` tool detects unreachable constraints or conflicting definitions within the schema itself, while `evaluate_schema_compatibility` identifies breaking changes when evolving your schemas.


## Available Tools (3)
- **evaluate_schema_compatibility**: Evaluates if a new schema is compatible with a base schema
- **lint_json_schema**: Performs structural linting on a JSON Schema
- **validate_json_document**: Validates a JSON document against a JSON Schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Schema Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this JSON document valid against my schema?"

**🤖 AI Agent:**
> The document is valid. No errors were found at any path.

---

**👤 You:**
> "Check this schema for any linting errors."

**🤖 AI Agent:**
> No structural or semantic errors were detected in the schema.

---

**👤 You:**
> "Will updating my schema break existing clients?"

**🤖 AI Agent:**
> No breaking changes were detected; the new schema is a valid superset of the base schema.


## ❓ FAQ

**Q: What does `validate_json_document` do?**
It checks a JSON document against a provided schema and returns validation errors with exact JSON Pointers.

**Q: How can I find logical errors in my schema?**
You can use the `lint_json_schema` tool to detect unreachable constraints or conflicting types within your schema definition.

**Q: Can I check if a new schema version breaks my existing integration?**
Yes, the `evaluate_schema_compatibility` tool compares a base schema with a new one to identify any breaking changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-schema-validator](https://vinkius.com/mcp/json-schema-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Schema Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-schema-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Schema Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-schema-validator": {
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
