# JSON Schema Validator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-schema-validator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json-schema-validator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json-schema-validator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Prevent malformed JSON hallucination. Validates large LLM-generated JSON objects strictly against JSON Schema standards before sending to the client.

## Description
Validating JSON against strict OpenAPI schemas is a mathematical task, not a probabilistic one. This engine uses `Ajv` for zero-hallucination validation.


## Available Tools
- **validate_json_schema**: Pass both as JSON strings. The engine returns whether the data is valid and lists all specific validation errors found.

Validates a JSON string optionally against a JSON Schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Schema Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this deeply nested JSON payload against our Draft-07 OpenAPI customer schema."

**🤖 AI Agent:**
> ✅ **Validation Status:** Valid.
All 34 fields comply with the expected type and constraint definitions.

---

**👤 You:**
> "Check if this user payload is missing any required properties according to the strict schema."

**🤖 AI Agent:**
> ❌ **Error Detected:**
`Missing required property 'billingAddress.zipCode' at root.user`

---

**👤 You:**
> "Ensure all strings in this array match the schema's maxLength of 50 characters."

**🤖 AI Agent:**
> ❌ **Validation Failed:** Item at index 4 (`companyName`) exceeds 50 characters.


## Installation & Usage

To install and use the **JSON Schema Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-schema-validator](https://vinkius.com/mcp/json-schema-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
