# Slug Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slug-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Transform any text into clean, SEO-friendly, URL-optimized slugs.

## Description
Slug Generator is an automated utility designed to transform arbitrary text strings into clean, URL-friendly, and SEO-optimized slugs. By removing noise, special characters, and accents, it ensures your URLs are compatible across all browsers and systems. Use `generate_slug` to create a sanitized slug from any input, or use `analyze_text_impact` to preview how much modification will occur. You can also use `list_active_stopwords` to see which words are currently eligible for removal during the process.


## Available Tools (3)
- **list_active_stopwords**: Retrieves the current inventory of active stopwords
- **analyze_text_impact**: Analyzes text to estimate the impact of the slugging process
- **generate_slug**: Returns the generated slug.

Converts a raw string into a sanitized, SEO-friendly slug


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slug Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 'Hello World! This is a Test.' into a slug."

**🤖 AI Agent:**
> hello-world-this-is-a-test

---

**👤 You:**
> "Generate a slug for 'Café & Restaurant' with stopword removal enabled."

**🤖 AI Agent:**
> cafe-restaurant

---

**👤 You:**
> "How much text will be modified in 'Check out this amazing 10% discount!'?"

**🤖 AI Agent:**
> The original length is 41 characters, with an estimated reduction of 5 characters due to sanitization.


## ❓ FAQ

**Q: What is a slug?**
A slug is the part of a URL that identifies a particular page in a human-readable format, typically consisting of lowercase letters, numbers, and hyphens.

**Q: How does the tool handle special characters?**
The tool automatically normalizes accented characters (like 'é' to 'e') and replaces all non-alphanumeric symbols with hyphens, ensuring a clean URL structure.

**Q: Can I remove common words like 'and' or 'the'?**
Yes, by setting the `applyStopwordRemoval` flag to true in the `generate_slug` tool, the engine will filter out predefined low-value tokens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slug-generator](https://vinkius.com/mcp/slug-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slug Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slug-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slug Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slug-generator": {
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
