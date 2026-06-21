# Weglot MCP Server

Automate website translation and localization — check API status, list supported languages, and translate text arrays directly via Weglot.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/weglot)

## Overview
**Category:** developer-tools
**Tools Count:** 4

## Description
Connect your **Weglot** account to any AI agent to streamline your multilingual content workflows. This MCP server provides direct access to Weglot's powerful translation engine, allowing for real-time localization and language management.

### What you can do

- **API Health Monitoring** — Use `get_status` to verify if the Weglot API is operational before running large translation batches.
- **Language Discovery** — Retrieve a comprehensive list of all languages supported by the Weglot platform using `list_languages`.
- **Pair Validation** — Confirm if specific translation directions (e.g., English to Japanese) are supported using `check_language_support`.
- **High-Volume Translation** — Translate arrays of sentences with full control over bot types and source URLs using the `translate_text` action.

### How it works

1. Subscribe to this server
2. Enter your Weglot API Key
3. Start translating content directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Managers** — quickly verify language support and test translations without leaving the chat interface.
- **Developers** — integrate translation checks into CI/CD pipelines or code editors to ensure content is ready for global deployment.
- **Content Creators** — instantly translate snippets or UI strings while maintaining context and metadata.


## Available Tools
- **check_language_support**: Check if a specific translation pair is supported
- **list_languages**: List all available languages supported by Weglot
- **get_status**: Do not spam this endpoint.

Check Weglot API status
- **translate_text**: Requires WEGLOT_API_KEY.

Translate an array of sentences


## Installation & Usage

To install and use the **Weglot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weglot](https://vinkius.com/mcp/weglot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
