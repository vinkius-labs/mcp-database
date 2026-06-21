# JSON Merge Patch MCP Server

Stop losing data when updating massive files. Apply surgical JSON patches (RFC 7396) securely to large datasets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/json-merge-patch)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
If an AI Agent needs to update just 3 fields in a 5,000-line JSON configuration file, asking the LLM to rewrite the entire file often leads to truncated data or forgotten keys due to context limits. This MCP solves that by shifting the merge logic to the Edge.

### The Superpowers

- **Surgical Updates:** The LLM only generates the 'patch' (what changed), and the V8 engine merges it flawlessly with the original file.
- **RFC 7396 Compliant:** Uses official industry standards for JSON merging, ensuring zero data corruption during the patch.


## Available Tools
- **apply_patch**: Pass the original and the patch as JSON strings. The engine applies deep merging deterministically.

Applies an RFC 7396 JSON Merge Patch deterministically. Allows LLMs to update massive JSON files by only sending the delta patch


## Installation & Usage

To install and use the **JSON Merge Patch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-merge-patch](https://vinkius.com/mcp/json-merge-patch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
