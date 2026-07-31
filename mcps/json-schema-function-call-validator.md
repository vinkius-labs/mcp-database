# JSON Schema Function Call Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-schema-function-call-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Verify that LLM-generated JSON function calls strictly adhere to your defined JSON Schemas.

## Description
The `validate_function_call` tool acts as a precision gate for AI agents. It parses raw LLM text outputs intended to be JSON function calls and validates them against any provided JSON Schema. The validator checks for missing required parameters, type mismatches (e.g., string vs integer), and hallucinated parameters not present in the schema. It returns exact error counts, a parameter validity percentage, and a strictly formatted error log, making it essential for building reliable agentic workflows.


## Available Tools (1)
- **validate_function_call**: Validates a JSON function call payload against a provided JSON Schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Schema Function Call Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this function call: {"name": "get_weather", "arguments": {"location": "London"}} against the schema {"type": "object", "properties": {"location": {"type": "string"}}, "required": ["location"]}"

**🤖 AI Agent:**
> Validation successful. The payload matches the schema perfectly.

---

**👤 You:**
> "Check if this call is valid: {"name": "add", "arguments": {"a": "5", "b": 10}} against schema {"type": "object", "properties": {"a": {"type": "integer"}, "b": {"type": "integer"}}, "required": ["a", "b"]}"

**🤖 AI Agent:**
> Validation failed. Error: Parameter 'a' expected type integer but received string.

---

**👤 You:**
> "Validate a call with an extra parameter: {"name": "resize", "arguments": {"width": 100, "height": 200, "format": "png"}} against schema {"type": "object", "properties": {"width": {"type": "integer"}, "height": {"type": "integer"}}, "required": ["width", "height"]}"

**🤖 AI Agent:**
> Validation failed. Error: Hallucinated parameter 'format' detected.


## ❓ FAQ

**Q: What does the validator check for?**
It checks for missing required parameters, type mismatches (like a string where an integer is expected), and hallucinated parameters that are not defined in your JSON Schema.

**Q: Can I use this to prevent hallucinations?**
Yes. By using `validate_function_call`, you can detect when an LLM attempts to use parameters that do not exist in your schema, allowing you to catch hallucinations before they reach your downstream logic.

**Q: What format should the input be in?**
The `payloadJson` and `schemaJson` must both be provided as valid JSON strings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-schema-function-call-validator](https://vinkius.com/mcp/json-schema-function-call-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Schema Function Call Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-schema-function-call-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Schema Function Call Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-schema-function-call-validator": {
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
