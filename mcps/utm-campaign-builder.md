# UTM Campaign Builder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/utm-campaign-builder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/utm-campaign-builder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/utm-campaign-builder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip Marketing Agents to generate flawless tracking links. Safely encode UTM parameters and prevent broken Google Analytics routing.

## Description
When a Martech AI Agent drafts social media posts or email campaigns, it needs to append tracking data to the links (UTMs). LLMs are notorious for hallucinating query strings—adding double `??`, forgetting to URL-encode spaces, or breaking existing parameters. This ruins data attribution in Google Analytics. This MCP solves that perfectly.

### The Superpowers

- **Strict URL Encoding:** Merges `utm_source`, `utm_medium`, and other parameters cleanly into any base URL using strict browser-grade encoding.
- **Analytics Protection:** Guarantees that every generated link works perfectly without causing 404s or dropping tracking data.


## Available Tools
- **build_utm_url**: Provide the base landing page URL, utm_source, and utm_medium as required fields. Optionally add campaign, term, and content. The engine handles all URL encoding and query string merging safely.

Safely constructs and encodes marketing UTM tracking URLs. Prevents AI from hallucinating broken query strings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UTM Campaign Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build a tracking URL for `https://vinkius.com/pricing` with source `linkedin` and medium `social`."

**🤖 AI Agent:**
> UTM Campaign URL: Generated successfully.

---

**👤 You:**
> "Add UTM tracking to this link for our Black Friday email blast."

**🤖 AI Agent:**
> UTM Campaign URL: Generated successfully.

---

**👤 You:**
> "I have this landing page that already has `?ref=affiliate`. Append the UTM source `facebook` safely."

**🤖 AI Agent:**
> UTM Campaign URL: Appended successfully.


## Installation & Usage

To install and use the **UTM Campaign Builder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/utm-campaign-builder](https://vinkius.com/mcp/utm-campaign-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
