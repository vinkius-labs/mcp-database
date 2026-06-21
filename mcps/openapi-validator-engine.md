# OpenAPI Validator Engine MCP Server

Validate any OpenAPI or Swagger spec (2.0, 3.0, 3.1, 3.2) local before generating code from it. Returns version, validity, and every schema error with exact paths. Your spec quality gate.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openapi-validator-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
Your agent is about to generate an SDK from an OpenAPI spec. But the spec has a missing `$ref`, an invalid schema type, and a path parameter that doesn't match the URL template. The generated code compiles but crashes at runtime. Nobody finds it until production.

This MCP validates OpenAPI/Swagger specifications against the official JSON Schema before any code generation happens. It catches every structural error with the exact path where it occurred.

### The Superpowers

- **4 Versions:** OpenAPI 2.0 (Swagger), 3.0, 3.1, and 3.2 — auto-detected.
- **Exact Error Paths:** Each error includes the JSON pointer (e.g. paths./users.get.responses.200.content) for surgical fixes.
- **Local:** No external API calls. The validation schema is embedded.
- **Quality Gate:** Use as a CI/CD gate — reject code generation from invalid specs.


## Available Tools
- **validate_openapi**: Pass the spec as a JSON string. The engine validates against the official OpenAPI JSON Schemas and returns all errors with paths. Supports Swagger 2.0, OpenAPI 3.0, 3.1, and 3.2.

Validates OpenAPI/Swagger specifications (2.0, 3.0.x, 3.1.x, 3.2.x) offline. Returns version, validity, and detailed error list


## Installation & Usage

To install and use the **OpenAPI Validator Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openapi-validator-engine](https://vinkius.com/mcp/openapi-validator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
