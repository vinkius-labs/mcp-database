# AI Token Counter MCP Server

Give AI Agents self-awareness of context limits. Count exact OpenAI/Claude tokens local to prevent fatal API truncation errors.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ai-token-counter)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
When a RAG Agent fetches 10 documents to summarize, it blindly sends them to the LLM API. If the payload exceeds the context window (e.g., 128k tokens), the API crashes, destroying the pipeline. LLMs cannot count their own tokens before sending a prompt. This MCP solves that perfectly.

### The Superpowers

- **Token Math:** Uses the exact `cl100k_base` encoding algorithm local to tell the Agent exactly how many tokens a payload contains.
- **Self-Aware Agents:** Allows Agents to do math and chunk their own massive datasets safely before hitting external API limits.


## Available Tools
- **count_tokens**: Pass the raw text and receive the exact token count. Use the result to decide whether to chunk, summarize, or send directly.

Counts exact LLM tokens (cl100k_base) offline. Prevents RAG agents from exceeding context windows and crashing


## Installation & Usage

To install and use the **AI Token Counter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ai-token-counter](https://vinkius.com/mcp/ai-token-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
