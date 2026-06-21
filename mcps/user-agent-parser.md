# User-Agent Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/user-agent-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/user-agent-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/user-agent-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Decode raw HTTP User-Agent strings instantly. Extract structured Browser, OS, and Device data for accurate IT log analysis.

## Description
When an IT Support Agent analyzes an error log or a firewall access log, it encounters messy User-Agent strings like `Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15`. LLMs often misinterpret these strings, causing them to hallucinate the wrong device or browser version. This MCP solves that entirely.

### The Superpowers

- **Deterministic Parsing:** Uses the industry-standard `ua-parser-js` to surgically extract the exact OS, Engine, Browser, and Device.
- **Log Analysis:** Transforms unreadable logs into clean JSON, empowering AI agents to accurately diagnose platform-specific bugs.


## Available Tools
- **parse_ua**: Pass the raw UA string from HTTP headers or server logs and receive exact identification of the client.

Decodes raw HTTP User-Agent strings into structured JSON objects (Browser, OS, Device). Prevents LLMs from hallucinating client specs from log files


## 💬 Prompt Examples

Here are some examples of how you can interact with the **User-Agent Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this UA from the server log: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7)`"

**🤖 AI Agent:**
> Parsed User-Agent: {"browser": {"name": "Chrome", "version": "114.0"}, "os": {"name": "Mac OS", "version": "10.15.7"}}

---

**👤 You:**
> "Find out what device the user is on based on this string: `Mozilla/5.0 (iPhone; CPU iPhone OS 16_5)`"

**🤖 AI Agent:**
> Parsed User-Agent: Device is Mobile, OS is iOS 16.5.

---

**👤 You:**
> "Extract the browser version from this Android User-Agent."

**🤖 AI Agent:**
> Result: Browser is Chrome version 120 on Android 13.


## Installation & Usage

To install and use the **User-Agent Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/user-agent-parser](https://vinkius.com/mcp/user-agent-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
