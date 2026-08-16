# Tool Call Schema Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tool-call-schema-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

High-precision validation of LLM tool call arguments against strict JSON Schema definitions.

## Description
Ensure runtime reliability for AI agents by strictly validating tool call arguments. This MCP server provides precise tools like `validate_tool_call` to check type conformity, numeric bounds, string lengths, and enum constraints. It performs deep, recursive traversal of complex nested objects and arrays, providing exact path-based error reporting (e.g., `args.user.id`) to pinpoint exactly where a schema violation occurs.


## Available Tools (3)
- **check_type_conformity**: Performs a granular check of a single value against a specific type constraint
- **summarize_validation_report**: Aggregates multiple validation errors into a human-readable summary for the user
- **validate_tool_call**: Checks if a specific set of tool arguments matches a provided schema definition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Call Schema Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate if these arguments match the schema: {"age": 25} with schema {"type": "object", "properties": {"age": {"type": "integer"}}, "required": ["age"]}"

**🤖 AI Agent:**
> The validation was successful.

---

**👤 You:**
> "Check if the value 10.5 matches the type 'integer'."

**🤖 AI Agent:**
> No, the value 10.5 is a number, not an integer.

---

**👤 You:**
> "Summarize these errors: [{"path": "args.name", "message": "is required"}]"

**🤖 AI Agent:**
> Validation failed: 1 error found. Path 'args.name': is required.


## ❓ FAQ

**Q: What does this tool validate?**
It validates that LLM-generated arguments strictly match a provided JSON Schema, including types, required fields, and logical constraints like min/max values.

**Q: How are errors reported?**
Errors are reported using precise path notation, such as `args.items[0].id`, so you know exactly which part of the input failed validation.

**Q: Can it handle nested objects?**
Yes, the validator uses recursive traversal to ensure every level of a nested object or array is checked against the schema.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tool-call-schema-validator](https://vinkius.com/ai-agent-connect/tool-call-schema-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Call Schema Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-call-schema-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Call Schema Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-call-schema-validator": {
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
