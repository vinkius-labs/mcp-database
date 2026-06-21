# Dot Object Transformer MCP Server

Flatten deeply nested JSON objects into dot-notation keys, or reconstruct nested objects from flat dictionaries.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dot-object-transformer)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
When an AI Agent needs to export nested API data to a CSV spreadsheet or rebuild a nested payload from flat form fields, it shouldn't guess the dot-notation mapping. This MCP handles it deterministically.

### The Superpowers

- **Bidirectional:** Flatten nested JSON to `{"user.name": "John"}` or unflatten it back.
- **Lossless:** Preserves arrays, nulls, and complex nested structures perfectly.


## Available Tools
- **transform_dot_object**: g. {"user.name": "John", "user.address.city": "NYC"}) for spreadsheet exports, or unflatten a flat dictionary back into a nested JSON structure for API payloads.

Flattens deeply nested JSON objects into single-level dot-notation keys, or reconstructs nested objects from flat dictionaries. Essential for CSV exports and API integrations


## Installation & Usage

To install and use the **Dot Object Transformer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dot-object-transformer](https://vinkius.com/mcp/dot-object-transformer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
