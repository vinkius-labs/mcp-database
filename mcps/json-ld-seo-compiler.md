# JSON-LD SEO Compiler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-ld-seo-compiler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Compile 100% Google-compliant JSON-LD Schema blocks. Prevent AI hallucination of invalid SEO structured data.

## Description
When a Martech AI Agent publishes an article or product to a CMS like WordPress, it often generates structured data (Rich Snippets). However, LLMs frequently hallucinate property names or forget mandatory attributes like `@context` and `@type`. Google rejects these invalid schemas. This MCP solves that perfectly.

### The Superpowers

- **Strict Construction:** Takes a simple JSON payload and deterministically injects all required Schema.org boilerplate to ensure Google compliance.
- **Zero Hallucination:** Outputs a perfectly formatted `<script type="application/ld+json">` block ready for direct HTML injection.


## Available Tools
- **build_schema**: Pass the Schema.org type (Article, Product, FAQPage, etc.) and a JSON string of properties. The engine injects @context and @type automatically and returns a valid <script type="application/ld+json"> block.

Compiles 100% compliant Google JSON-LD schema blocks for SEO. Prevents AI hallucination of invalid @context or @type attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON-LD SEO Compiler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build a JSON-LD snippet for an `Article` with this metadata: `{"headline": "AI Agents 2026", "author": "John Doe"}`"

**🤖 AI Agent:**
> JSON-LD SEO Schema: Block generated successfully.

---

**👤 You:**
> "Compile this product data into a Google-compliant structured data format."

**🤖 AI Agent:**
> JSON-LD SEO Schema: The application/ld+json script is ready.

---

**👤 You:**
> "Generate an FAQPage schema for these three questions."

**🤖 AI Agent:**
> JSON-LD SEO Schema: Compiled successfully.


## ❓ FAQ

**Q: Why do I need an engine for this?**
LLMs can easily break JSON syntax (missing quotes, trailing commas) which causes HTML parsers to crash. This engine parses and stringifies deterministically.

**Q: Does it support all Schema types?**
Yes! You can pass any valid Schema.org type like `Article`, `Product`, `FAQPage`, or `LocalBusiness`.

**Q: Can it nest objects?**
Yes, just pass a nested JSON payload and the engine will compile it correctly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-ld-seo-compiler](https://vinkius.com/mcp/json-ld-seo-compiler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON-LD SEO Compiler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `json-ld-seo-compiler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON-LD SEO Compiler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-ld-seo-compiler": {
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
