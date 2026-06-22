# Heading Structure Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heading-structure-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Validates HTML heading hierarchy, keyword presence, and semantic density.

## Description
An MCP server designed to audit webpage document outlines. It ensures structural integrity by checking for proper H1-H6 nesting, verifies the presence of target keywords in headings, and calculates semantic density to measure information richness across different heading levels. Use `check_hierarchy` to detect skipped levels or multiple H1s, `verify_keywords` to ensure SEO compliance, and `calculate_semantic_density` to assess content variety.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heading Structure Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this list of headings has any hierarchy errors: [{'level': 'h1', 'text': 'Title'}, {'level': 'h3', 'text': 'Subtitle'}]"

**🤖 AI Agent:**
> The hierarchy is invalid because an H3 follows an H1, skipping the H2 level.

---

**👤 You:**
> "Are the keywords 'SEO' and 'HTML' present in my headings?"

**🤖 AI Agent:**
> Yes, both 'SEO' and 'HTML' were found in your heading structure.

---

**👤 You:**
> "Calculate the semantic density for these headings: [{'level': 'h1', 'text': 'Main Title'}, {'level': 'h2', 'text': 'Section 1'}]"

**🤖 AI Agent:**
> The density score for h1 is 1.0 and for h2 is 1.0.


## ❓ FAQ

**Q: How do I check for heading hierarchy errors?**
Use the `check_hierarchy` tool by providing an array of objects containing the level and text of your headings. Tools available: `your_tool_name`.

**Q: Can I verify specific keywords in my H2 tags?**
Yes, use `verify_keywords` and specify the target level as 'h2' to check for your required terms.

**Q: What is semantic density?**
It is a measure of how much unique, meaningful information is present in each heading level compared to the total word count, calculated via `calculate_semantic_density`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heading-structure-validator](https://vinkius.com/mcp/heading-structure-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heading Structure Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heading-structure-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heading Structure Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heading-structure-validator": {
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
