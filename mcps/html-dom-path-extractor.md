# HTML DOM Path Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/html-dom-path-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate precise CSS selectors and XPath strings from raw HTML strings.

## Description
The HTML DOM Path Extractor is a specialized tool for web scraping and automation workflows. It parses raw HTML strings to generate exact CSS selectors or XPath strings for specified elements without requiring a browser environment. The engine performs strict string tokenization, stripping away inline scripts and styles to ensure clean data extraction. Beyond path generation, it provides structural insights by counting exact tag frequencies and validating the integrity of tag closures (e.g., detecting unmatched  tags). This makes it an essential component for building reliable web scrapers and automated testing suites that need to navigate complex DOM structures accurately.


## Available Tools (1)
- **extract_html_paths**: The tool will strip scripts/styles, validate tags, and return extracted paths and frequencies.

Parses raw HTML and generates CSS selectors, XPath strings, and tag frequencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML DOM Path Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract paths from this HTML: <div><p id='test'>Hello</p></div>"

**🤖 AI Agent:**
> CSS Selector: div p#test, XPath: /div/p[@id='test'], Tag Frequencies: div: 1, p: 1

---

**👤 You:**
> "Check if this HTML has unclosed tags: <div><span>Content</div>"

**🤖 AI Agent:**
> Validation Error: Unmatched <span> tag detected. The structure is incomplete.

---

**👤 You:**
> "What are the tag frequencies in: <ul><li class='item'>Item 1</li><li class='item'>Item 2</li></ul>"

**🤖 AI Agent:**
> Tag Frequencies: ul: 1, li: 2


## ❓ FAQ

**Q: Does this tool require a browser like Chrome or Firefox?**
No, the `extract_html_paths` tool uses strict string tokenization to parse HTML, making it extremely fast and lightweight without needing a headless browser.

**Q: Can it detect broken or unclosed HTML tags?**
Yes, one of the core features is validating tag closure integrity, which helps identify unmatched tags like <div> or <span> in your input string.

**Q: How does it handle scripts and styles within the HTML?**
The tool automatically strips inline <script> and <style> tags during the parsing process to ensure that the generated paths and tag frequencies only reflect the visible DOM structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/html-dom-path-extractor](https://vinkius.com/ai-agent-connect/html-dom-path-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTML DOM Path Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `html-dom-path-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTML DOM Path Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html-dom-path-extractor": {
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
