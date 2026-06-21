# UTM Campaign Builder MCP Server

Equip Marketing Agents to generate flawless tracking links. Safely encode UTM parameters and prevent broken Google Analytics routing.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/utm-campaign-builder)

## Overview
**Category:** marketing-automation
**Tools Count:** 1

## Description
When a Martech AI Agent drafts social media posts or email campaigns, it needs to append tracking data to the links (UTMs). LLMs are notorious for hallucinating query strings—adding double `??`, forgetting to URL-encode spaces, or breaking existing parameters. This ruins data attribution in Google Analytics. This MCP solves that perfectly.

### The Superpowers

- **Strict URL Encoding:** Merges `utm_source`, `utm_medium`, and other parameters cleanly into any base URL using strict browser-grade encoding.
- **Analytics Protection:** Guarantees that every generated link works perfectly without causing 404s or dropping tracking data.


## Available Tools
- **build_utm_url**: Provide the base landing page URL, utm_source, and utm_medium as required fields. Optionally add campaign, term, and content. The engine handles all URL encoding and query string merging safely.

Safely constructs and encodes marketing UTM tracking URLs. Prevents AI from hallucinating broken query strings


## Installation & Usage

To install and use the **UTM Campaign Builder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/utm-campaign-builder](https://vinkius.com/mcp/utm-campaign-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
