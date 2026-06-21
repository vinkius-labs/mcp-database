# HTML DOM Query Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-dom-query-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Extract specific text and attributes from massive HTML payloads instantly using CSS selectors. Fast, memory-efficient DOM parsing.

## Description
If an AI agent needs to scrape a product price from a 20,000-line e-commerce HTML page, passing the entire raw HTML to the LLM destroys its token limit and leads to hallucination. This MCP allows the LLM to pass the raw string and a CSS selector, instantly returning just the target data.

### The Superpowers

- **Token Saver:** Offloads heavy DOM parsing to the native V8 runtime via Cheerio.
- **Precision Scraping:** Supports complex CSS selectors (e.g. `#main .price`) and extracts specific attributes like `href` or `src`.


## Available Tools
- **query_dom**: Pass the HTML string and a CSS query (e.g. "h1", ".price", "#title"). Returns the matched text content or attributes.

Parses a raw HTML string and extracts text or attributes using a CSS selector deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML DOM Query Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the text from `.product-price` from this 5,000 line HTML file."

**🤖 AI Agent:**
> ✅ **Matches Found:**
1. `$149.99`

---

**👤 You:**
> "Extract all image source URLs (`src`) from the `.gallery img` selector."

**🤖 AI Agent:**
> ✅ **Matches:** Extracted 12 `src` attributes successfully.

---

**👤 You:**
> "Get the text inside the `<h1>` tag."

**🤖 AI Agent:**
> ✅ **Matched Text:** 'Welcome to our API documentation.'


## ❓ FAQ

**Q: Does it download the URL?**
No, it parses raw HTML strings that you pass to it.

**Q: Can it extract link URLs?**
Yes, just pass 'href' in the attribute parameter.

**Q: Is it fast?**
Yes, it uses Cheerio, which runs entirely in memory without a headless browser.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-dom-query-engine](https://vinkius.com/mcp/html-dom-query-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTML DOM Query Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `html-dom-query-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTML DOM Query Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html-dom-query-engine": {
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
