# User-Agent Parser MCP Server

Decode raw HTTP User-Agent strings instantly. Extract structured Browser, OS, and Device data for accurate IT log analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/user-agent-parser)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
When an IT Support Agent analyzes an error log or a firewall access log, it encounters messy User-Agent strings like `Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15`. LLMs often misinterpret these strings, causing them to hallucinate the wrong device or browser version. This MCP solves that entirely.

### The Superpowers

- **Deterministic Parsing:** Uses the industry-standard `ua-parser-js` to surgically extract the exact OS, Engine, Browser, and Device.
- **Log Analysis:** Transforms unreadable logs into clean JSON, empowering AI agents to accurately diagnose platform-specific bugs.


## Available Tools
- **parse_ua**: Pass the raw UA string from HTTP headers or server logs and receive exact identification of the client.

Decodes raw HTTP User-Agent strings into structured JSON objects (Browser, OS, Device). Prevents LLMs from hallucinating client specs from log files


## Installation & Usage

To install and use the **User-Agent Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/user-agent-parser](https://vinkius.com/mcp/user-agent-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
