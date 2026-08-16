# XPath Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/xpath-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-scraping](../categories/web-scraping.md)

Extract precise data from XML and HTML using XPath 1.0 expressions.

## Description
XPath Extractor provides precise tools for navigating and querying XML and HTML documents. Use `evaluate_xpath_expression` to retrieve specific node values or attribute strings, `validate_document_structure` to ensure your documents are well-formed, and `extract_node_attributes` to pull specific attribute values from matched elements. This connector bridges your AI agent to structured data parsing logic.


## Available Tools (3)
- **evaluate_xpath_expression**: Executes an XPath 1.0 query against a provided document string to retrieve specific data
- **extract_node_attributes**: Specifically targets and retrieves the values of attributes within a set of nodes
- **validate_document_structure**: Checks if a provided string adheres to structural rules and identifies syntax errors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **XPath Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the value of the 'id' attribute from the first 'div' element in this HTML: <div><p id='main'>Hello</p></div>"

**🤖 AI Agent:**
> main

---

**👤 You:**
> "What is the text content of the 'title' tag in this XML? <root><title>Example Title</title></root>"

**🤖 AI Agent:**
> Example Title

---

**👤 You:**
> "Check if this XML is valid: <root><item>Data</item></root>"

**🤖 AI Agent:**
> true


## ❓ FAQ

**Q: What kind of documents can I parse?**
You can parse both XML and HTML documents. Use `validate_document_structure` to check if your document is well-formed before running queries.

**Q: How do I get attribute values?**
You can use `extract_node_attributes` to target specific attributes, or use `evaluate_xpath_expression` with an XPath expression that points directly to the attribute.

**Q: Does it support HTML5?**
The tool supports HTML parsing via the 'html' mode in `validate_document_structure`, which is more lenient with unclosed tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/xpath-extractor](https://vinkius.com/ai-agent-connect/xpath-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **XPath Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `xpath-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **XPath Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "xpath-extractor": {
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
