# JSON-LD SEO Compiler MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-ld-seo-compiler)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json-ld-seo-compiler-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json-ld-seo-compiler-mcp)
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


## Installation & Usage

To install and use the **JSON-LD SEO Compiler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-ld-seo-compiler](https://vinkius.com/mcp/json-ld-seo-compiler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
