# URL Slug Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-slug-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data](../categories/data.md)

Transliterate complex international text into 100% SEO-friendly URL slugs. Prevent AI hallucination of invalid characters in CMS routing.

## Description
When Marketing AI Agents publish blog posts or e-commerce products, they need to generate a URL slug from the title (e.g., `Ação e Coração!` -> `acao-e-coracao`). LLMs frequently fail at this by leaving in diacritics, double dashes, or invalid Unicode characters, causing 404 errors and broken SEO. This MCP solves that perfectly.

### The Superpowers

- **Strict Transliteration:** Uses `slugify` to deterministically strip accents, emojis, and special symbols from any language.
- **SEO Perfection:** Ensures all slugs are lowercase, safely hyphenated, and perfectly formatted for Google and CMS platforms.


## Available Tools
- **validate_cron_expression**: Pass the 5-field cron string (e.g. "0 9 * * 1-5") and receive validation status with field-level error diagnostics.

Validates cron expressions by checking field ranges, step values, and syntax correctness offline


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


## ❓ FAQ

**Q: Does it support non-Latin languages?**
Yes, it intelligently transliterates Cyrillic, Arabic, Vietnamese, and more into safe Latin characters.

**Q: Will it leave trailing hyphens?**
No, it is strictly configured to trim trailing hyphens and prevent double-hyphens.

**Q: Why use an MCP for this?**
Because LLMs hallucinate URL encoding. Passing it through a deterministic V8 engine guarantees a 0% error rate for your CMS routing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-slug-generator](https://vinkius.com/mcp/url-slug-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL Slug Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `url-slug-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL Slug Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-slug-generator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
