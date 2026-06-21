# JSON Path Query Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-path-query-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json-path-query-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json-path-query-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Extract specific data from massive JSON payloads using JSONPath expressions.

## Description
Surgically extract fields from complex API responses using JSONPath Plus (8M+ weekly downloads). Saves tokens and prevents hallucination.

### The Superpowers

- **Surgical Extraction:** Full JSONPath syntax (`$.orders[0].total_price`, `$..email`).
- **Token Efficient:** Extract only the 3 fields you need from a 5,000-token payload.


## Available Tools
- **query_json**: Pass the raw JSON string and a JSONPath expression like "$.orders[0].total_price" or "$.users[*].email". Returns all matching values.

Queries and extracts specific values from massive JSON payloads using JSONPath expressions. Eliminates the need to send entire API responses to the LLM context window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Path Query Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract all author names from this bookstore JSON."

**🤖 AI Agent:**
> JSONPath Result: 4 matches found.


## Installation & Usage

To install and use the **JSON Path Query Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-path-query-engine](https://vinkius.com/mcp/json-path-query-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
