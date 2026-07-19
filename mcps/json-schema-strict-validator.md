# JSON Schema Strict Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-schema-strict-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Perform deterministic JSON validation against Draft-07 and 2020-12 schemas with strict property enforcement.

## Description
This MCP server provides a zero-tolerance validation engine for JSON data. It ensures that your JSON instances strictly adhere to defined schemas by enforcing rules like `additionalProperties: false` by default. Use `validate_json` to check for type mismatches, missing required fields, or pattern failures. The `verify_integrity` tool allows you to validate environment variable strings against expected types, while `evaluate_compatibility` detects breaking changes between schema versions. It is ideal for preventing subtle schema violations in automated pipelines.


## Available Tools (3)
- **validate_json**: The engine will parse them and perform strict validation, including checking for additional properties if specified.

Validates a JSON instance against a provided JSON Schema
- **verify_integrity**: ) and a JSON array of constraints [{key, expectedType}].

Verifies that environment variables or a string of key-value pairs match expected types
- **evaluate_compatibility**: Evaluates if a new JSON Schema is compatible with an old one


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Schema Strict Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this JSON object against the schema: {"name": "John", "age": 30} with schema {"type": "object", "properties": {"name": {"type": "string"}}, "required": ["name"]}"

**🤖 AI Agent:**
> {"isValid": true, "validationErrors": []}

---

**👤 You:**
> "Check if this JSON is valid: {"id": 123, "extra": true} against schema {"type": "object", "properties": {"id": {"type": "number"}}}"

**🤖 AI Agent:**
> {"isValid": false, "validationErrors": [{"path": "/extra", "errorType": "UNAUTHORIZED_PROPERTY", "expected": "none", "actual": "true"}]}

---

**👤 You:**
> "Is the string 'VERSION=1.0' valid for the key VERSION with type string?"

**🤖 AI Agent:**
> {"isHealthy": true, "structuralIssues": []}


## ❓ FAQ

**Q: What does 'strict mode' mean in this validator?**
Strict mode means that if a schema does not explicitly define `additionalProperties`, the validator treats it as `false`. Any property found in the JSON instance that is not declared in the schema will trigger an error.

**Q: Can I use this to check for breaking changes in my API?**
Yes, by using the `evaluate_compatibility` tool, you can compare an old schema against a new one to identify removed required fields or properties that might break your integration.

**Q: How do I validate environment variables?**
You can use the `verify_integrity` tool. Pass a string of key-value pairs (like `PORT=8080`) and an array of constraints to ensure each key matches its expected type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-schema-strict-validator](https://vinkius.com/mcp/json-schema-strict-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Schema Strict Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-schema-strict-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Schema Strict Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-schema-strict-validator": {
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
