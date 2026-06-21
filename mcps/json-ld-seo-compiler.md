# JSON-LD SEO Compiler MCP Server

Compile 100% Google-compliant JSON-LD Schema blocks. Prevent AI hallucination of invalid SEO structured data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/json-ld-seo-compiler)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
When a Martech AI Agent publishes an article or product to a CMS like WordPress, it often generates structured data (Rich Snippets). However, LLMs frequently hallucinate property names or forget mandatory attributes like `@context` and `@type`. Google rejects these invalid schemas. This MCP solves that perfectly.

### The Superpowers

- **Strict Construction:** Takes a simple JSON payload and deterministically injects all required Schema.org boilerplate to ensure Google compliance.
- **Zero Hallucination:** Outputs a perfectly formatted `<script type="application/ld+json">` block ready for direct HTML injection.


## Available Tools
- **build_schema**: Pass the Schema.org type (Article, Product, FAQPage, etc.) and a JSON string of properties. The engine injects @context and @type automatically and returns a valid <script type="application/ld+json"> block.

Compiles 100% compliant Google JSON-LD schema blocks for SEO. Prevents AI hallucination of invalid @context or @type attributes


## Installation & Usage

To install and use the **JSON-LD SEO Compiler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-ld-seo-compiler](https://vinkius.com/mcp/json-ld-seo-compiler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
