# JSON Schema Function Call Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-schema-function-call-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validates raw LLM text outputs against JSON Schemas to detect missing parameters, type mismismatches, and hallucinations.

## Description
This MCP server provides essential tools for LLM orchestration and reliability. It allows agents to parse messy text outputs and validate them against strict JSON Schemas. Use `validate_function_call` to identify missing required parameters, type mismatches, or hallucinated keys. The `extract_json_from_text` tool helps isolate JSON blocks from conversational filler, while `get_validation_summary` provides high-level reliability metrics across multiple attempts. This is critical for ensuring that AI agents follow structured function-calling protocols accurately.


## Available Tools (3)
- **extract_json_from_text**: A utility to isolate the JSON component from a messy LLM text string
- **get_validation_summary**: Provides a high-level overview of multiple validation attempts to track model reliability over time
- **validate_function_call**: Validates a raw LLM text string against a specific JSON Schema to identify structural and logical errors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Schema Function Call Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this LLM output: 'Here is the call: {"action": "get_weather", "city": 123}' against a schema where city must be a string."

**🤖 AI Agent:**
> {"missingCount": 0, "typeMismatchCount": 1, "hallucinationCount": 0, "validityPercentage": 50.0, "errorLog": ["Parameter 'city' expected type string, but received integer."]}

---

**👤 You:**
> "Extract the JSON from this text: 'Sure! Here is your data: {"id": 1, "name": "test"} hope this helps!'"

**🤖 AI Agent:**
> {"id": 1, "name": "test"}

---

**👤 You:**
> "Check if this function call is valid: {"user_id": "abc-123"} using a schema that requires 'user_id' and 'session_id'."

**🤖 AI Agent:**
> {"missingCount": 1, "typeMismatchCount": 0, "hallucinationCount": 0, "validityPercentage": 50.0, "errorLog": ["Missing required parameter: session_id"]}


## ❓ FAQ

**Q: How does the validator handle conversational text around the JSON?**
The `extract_json_from_text` tool specifically isolates the JSON block by finding the first and last curly braces, allowing the validator to ignore surrounding markdown or conversational filler.

**Q: What kind of errors does `validate_function_call` detect?**
It detects three main error types: missing required parameters, type mismatches (e.g., a string where an integer is expected), and hallucinations (parameters present in the output but not in the schema).

**Q: Can I track the reliability of my LLM over time?**
Yes, you can use `get_validation_summary` by providing a history of previous validation results to calculate average validity and a qualitative reliability rating.


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
