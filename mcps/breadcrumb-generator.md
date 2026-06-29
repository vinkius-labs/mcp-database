# Breadcrumb Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/breadcrumb-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Automatically generates text, JSON-LD schema, and HTML breadcrumbs from URL paths.

## Description
The Breadcrumb Generator MCP server automates the creation of structural breadcrumbs in plain text, JSON-LD schema, and HTML formats. By providing a structured URL path, you can instantly obtain SEO-ready markup for search engines or accessible navigation elements for web interfaces. Use `generate_text_breadcrumb` for simple visual trails, `generate_json_ld_schema` to enhance your site's visibility in search results via Schema.org, and `generate_html_breadcrumb` to produce semantic HTML5 `` elements with relative links.


## Available Tools (3)
- **generate_html_breadcrumb**: Generates an HTML breadcrumb snippet
- **generate_json_ld_schema**: Generates a JSON-LD schema for BreadcrumbList
- **generate_text_breadcrumb**: Generates a plain text breadcrumb


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breadcrumb Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a text breadcrumb for the path '/clothing/men/shirts'."

**🤖 AI Agent:**
> Home > Clothing > Men > Shirts

---

**👤 You:**
> "Create a JSON-LD schema for '/services/consulting/strategy'."

**🤖 AI Agent:**
> {"@context": "https://schema.org", "@type": "BreadcrumbList", "itemListElement": [{"@type": "ListItem", "position": 1, "name": "Home", "item": "/"}, {"@type": "ListItem", "position": 2, "name": "Services", "item": "/services"}, {"@type": "ListItem", "position": 3, "name": "Consulting", "item": "/services/consulting"}, {"@type": "ListItem", "position": 4, "name": "Strategy", "item": "/services/consulting/strategy"}]}

---

**👤 You:**
> "Generate HTML breadcrumb markup for '/blog/news/updates'."

**🤖 AI Agent:**
> <nav aria-label="Breadcrumb"><ul class="breadcrumb"><li><a href="/">Home</a></li><li><a href="/blog">Blog</a></li><li><a href="/blog/news">News</a></li><li>Updates</li></ul></nav>


## ❓ FAQ

**Q: What formats can the breadcrumb generator produce?**
It produces three formats: plain text for simple visual trails, JSON-LD schema for SEO optimization, and semantic HTML5 markup for web navigation.

**Q: How do I provide the URL path?**
You simply pass the URL path string (e.g., '/products/electronics/mobile') as the `urlPath` parameter to any of the available tools.

**Q: Does the HTML output include links?**
Yes, the `generate_html_breadcrumb` tool generates an unordered list where each segment (except the current page) is wrapped in a relative anchor tag.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/breadcrumb-generator](https://vinkius.com/mcp/breadcrumb-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breadcrumb Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breadcrumb-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breadcrumb Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breadcrumb-generator": {
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
