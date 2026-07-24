# HTML DOM Path Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-dom-path-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate robust, deterministic CSS selectors from HTML snippets to prevent brittle web scraping.

## Description
The HTML DOM Path Generator is a specialized MCP server designed to solve the problem of fragile web scrapers. By providing an HTML snippet and a target element ID, it uses deterministic tree traversal to calculate exact CSS paths using nth-of-type indices. The engine prioritizes IDs, then unique classes, and finally structural paths. You can use generate_css_selector to find precise paths, validate_selector_integrity to ensure selector accuracy, and get_selector_complexity to assess how stable your selectors are against UI changes.


## Available Tools (3)
- **generate_css_selector**: Generates a CSS selector for an element with a specific ID within an HTML snippet
- **get_selector_complexity**: Calculates a complexity score for a CSS selector
- **validate_selector_integrity**: Validates if a CSS selector correctly resolves to an element in the provided HTML


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML DOM Path Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a CSS selector for the element with ID 'submit-btn' in this HTML: '<div class="container"><button id="submit-btn" class="primary">Click Me</button></div>'"

**🤖 AI Agent:**
> #submit-btn

---

**👤 You:**
> "How complex is the selector 'div:nth-of-type(2) > p:nth-of-type(1)'?"

**🤖 AI Agent:**
> The complexity score is 7. Factors include deep nesting and reliance on structural nth-of-type positioning.

---

**👤 You:**
> "Validate if the selector 'ul > li:nth-child(2)' is valid for this HTML: '<ul><li>Item 1</li><li>Item 2</li></ul>'"

**🤖 AI Agent:**
> The selector is valid and matches 1 element in the provided snippet.


## ❓ FAQ

**Q: How does the tool ensure selectors are not brittle?**
The engine uses a strict hierarchy: it first looks for an ID, then checks for unique classes within the sibling context, and only falls back to structural nth-of-type selectors when necessary. This minimizes reliance on deep nesting.

**Q: Can I use this for any HTML fragment?**
Yes, the tool is designed to parse HTML snippets or fragments. As long as the target element and its necessary parent context are included in the snippet, generate_css_selector will work correctly.

**Q: What is a complexity score?**
A complexity score from 1 to 10 indicates how likely a selector is to break. A score of 1 means it uses an ID and is highly stable, while higher scores indicate reliance on deep structural paths.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-dom-path-generator](https://vinkius.com/mcp/html-dom-path-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTML DOM Path Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `html-dom-path-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTML DOM Path Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html-dom-path-generator": {
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
