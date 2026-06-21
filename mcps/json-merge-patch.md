# JSON Merge Patch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-merge-patch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json-merge-patch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json-merge-patch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop losing data when updating massive files. Apply surgical JSON patches (RFC 7396) securely to large datasets.

## Description
If an AI Agent needs to update just 3 fields in a 5,000-line JSON configuration file, asking the LLM to rewrite the entire file often leads to truncated data or forgotten keys due to context limits. This MCP solves that by shifting the merge logic to the Edge.

### The Superpowers

- **Surgical Updates:** The LLM only generates the 'patch' (what changed), and the V8 engine merges it flawlessly with the original file.
- **RFC 7396 Compliant:** Uses official industry standards for JSON merging, ensuring zero data corruption during the patch.


## Available Tools
- **apply_patch**: Pass the original and the patch as JSON strings. The engine applies deep merging deterministically.

Applies an RFC 7396 JSON Merge Patch deterministically. Allows LLMs to update massive JSON files by only sending the delta patch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Merge Patch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Merge this patch `{"status": "active"}` into the 3MB user database JSON."

**🤖 AI Agent:**
> ✅ **Patched Output:** Output cleanly updated without touching other keys.

---

**👤 You:**
> "Remove the `temporary_token` key from this payload by applying a null patch."

**🤖 AI Agent:**
> ✅ **Applied:** Key successfully deleted per RFC 7396 standard.


## Installation & Usage

To install and use the **JSON Merge Patch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-merge-patch](https://vinkius.com/mcp/json-merge-patch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
