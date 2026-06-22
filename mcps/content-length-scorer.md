# Content Length Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/content-length-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Analyze text word counts against industry-standard length benchmarks based on content intent.

## Description
The Content Length Scorer is an analytical tool that evaluates if your writing meets the ideal word count boundaries for specific formats. By using tools like `analyze_content_compliance`, you can determine if a piece of text is 'BELOW', 'OPTIMATIONS', or 'EXCESSIVE' relative to its intended purpose, such as micro-copy, standard descriptions, extended landing pages, or pillar blog posts. Use `get_type_thresholds` to reveal the target word count ranges and `list_supported_intents` to see all available content categories.


## Available Tools (3)
- **analyze_content_compliance**: Evaluates if a specific piece of text meets the length requirements for its intended purpose
- **get_type_thresholds**: Retrieves the specific minimum and maximum word count targets for a given content type
- **list_supported_intents**: Provides a full list of all content types that the scorer can analyze


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Content Length Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this text optimal for a micro content type: 'Welcome to our new store!'?"

**🤖 AI Agent:**
> The word count is 6. For the micro category, this falls within the optimal range.

---

**👤 You:**
> "Check if a 500-word blog post is too long for the pillar category."

**🤖 AI Agent:**
> A 500-word count for a pillar content type is classified as BELOW the optimal range.

---

**👤 You:**
> "What are the word count boundaries for standard content?"

**🤖 AI Agent:**
> For the standard content type, the optimal range is between 50 and 250 words.


## ❓ FAQ

**Q: How does the compliance check work?**
The `analyze_content_compliance` tool counts every individual word in your provided text and compares that total against predefined minimum and maximum thresholds for the chosen content type.

**Q: What are the supported content types?**
You can analyze four main categories: `micro` for short snippets, `standard` for descriptions, `extended` for landing pages, and `pillar` for long-form guides. Use `list_supported_intents` to see the full registry.

**Q: Can I see the specific word count targets?**
Yes, use the `get_type_thresholds` tool by providing a content type to retrieve the exact minimum and maximum word count boundaries for that category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/content-length-scorer](https://vinkius.com/mcp/content-length-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Content Length Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `content-length-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Content Length Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "content-length-scorer": {
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
