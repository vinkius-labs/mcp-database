# URL Slug Generator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-slug-generator-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/url-slug-generator-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/url-slug-generator-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Transliterate complex international text into 100% SEO-friendly URL slugs. Prevent AI hallucination of invalid characters in CMS routing.

## Description
When Marketing AI Agents publish blog posts or e-commerce products, they need to generate a URL slug from the title (e.g., `Ação e Coração!` -> `acao-e-coracao`). LLMs frequently fail at this by leaving in diacritics, double dashes, or invalid Unicode characters, causing 404 errors and broken SEO. This MCP solves that perfectly.

### The Superpowers

- **Strict Transliteration:** Uses `slugify` to deterministically strip accents, emojis, and special symbols from any language.
- **SEO Perfection:** Ensures all slugs are lowercase, safely hyphenated, and perfectly formatted for Google and CMS platforms.


## Available Tools
- **generate_slug**: Pass the raw title or text and receive a properly transliterated, lowercase, hyphenated slug safe for any URL. Handles international characters like accents and CJK.

Transliterates complex international text into 100% SEO-friendly URL slugs. Prevents AI hallucination of invalid characters in CMS routing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL Slug Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a URL slug for this article title: `Ação e Coração! O Guia Definitivo 2026.`"

**🤖 AI Agent:**
> Generated URL Slug: `acao-e-coracao-o-guia-definitivo-2026`

---

**👤 You:**
> "Turn this weird string `My Awesome   Product --- 100% Good` into a clean SEO slug."

**🤖 AI Agent:**
> Generated URL Slug: `my-awesome-product-100-good`

---

**👤 You:**
> "Create a URL-safe route for the category `café & bistrô`."

**🤖 AI Agent:**
> Generated URL Slug: `cafe-bistro`


## Installation & Usage

To install and use the **URL Slug Generator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-slug-generator-alternative](https://vinkius.com/mcp/url-slug-generator-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
