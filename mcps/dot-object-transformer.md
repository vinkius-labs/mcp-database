# Dot Object Transformer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dot-object-transformer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dot-object-transformer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dot-object-transformer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Flatten deeply nested JSON objects into dot-notation keys, or reconstruct nested objects from flat dictionaries.

## Description
When an AI Agent needs to export nested API data to a CSV spreadsheet or rebuild a nested payload from flat form fields, it shouldn't guess the dot-notation mapping. This MCP handles it deterministically.

### The Superpowers

- **Bidirectional:** Flatten nested JSON to `{"user.name": "John"}` or unflatten it back.
- **Lossless:** Preserves arrays, nulls, and complex nested structures perfectly.


## Available Tools
- **transform_dot_object**: g. {"user.name": "John", "user.address.city": "NYC"}) for spreadsheet exports, or unflatten a flat dictionary back into a nested JSON structure for API payloads.

Flattens deeply nested JSON objects into single-level dot-notation keys, or reconstructs nested objects from flat dictionaries. Essential for CSV exports and API integrations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dot Object Transformer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Flatten this nested user profile JSON for CSV export."

**🤖 AI Agent:**
> Dot Object Result: 8 keys flattened.


## Installation & Usage

To install and use the **Dot Object Transformer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dot-object-transformer](https://vinkius.com/mcp/dot-object-transformer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
