# Language Detector Engine MCP Server

Detect the language of any text local using exact n-gram analysis. Supports 400+ languages. When AI guesses wrong on short or mixed text, this engine proves it.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/language-detector-engine)

## Overview
**Category:** customer-support
**Tools Count:** 1

## Description
Your customer support agent receives a ticket: 'O produto não chegou'. The AI routes it to the Spanish queue. The agent wastes time, the customer gets angry, SLA drops. Why? Because the AI 'guessed' the language probabilistically instead of calculating it.

This MCP uses `franc` (200K+ weekly downloads, inspired by Google's CLD2) to perform deterministic N-gram language detection. It returns exact ISO 639-3 codes for over 400 languages, and properly returns 'undefined' if a text is too ambiguous rather than hallucinating.

### The Superpowers

- **400+ Languages:** From English (eng) and Portuguese (por) to Esperanto (epo) and Zulu (zul).
- **Exact N-gram Math:** Analyzes text strictly by character frequencies, not LLM probability.
- **Whitelist/Blacklist:** Know the text must be either Spanish or Portuguese? Pass `only: ['spa', 'por']` to force a strict evaluation.
- **Confidence Scores:** Use the `all` flag to get an array of all matches with their exact probability scores.


## Available Tools
- **detect_language**: Provide as much text as possible for higher accuracy.

Detect the language of any text using n-gram analysis. Supports 400+ languages. Returns ISO 639-3 codes (e.g., "por", "eng", "spa")


## Installation & Usage

To install and use the **Language Detector Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/language-detector-engine](https://vinkius.com/mcp/language-detector-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
