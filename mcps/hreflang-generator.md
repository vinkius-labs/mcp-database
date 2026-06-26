# Hreflang Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hreflang-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Generate and validate SEO-compliant HTML hreflang tags and XML sitemap entries for multi-regional websites.

## Description
The Hreflang Generator is a specialized utility designed to manage internationalized SEO. It automates the creation of HTML `` tags and XML sitemap entries, ensuring that every URL in your regional cluster maintains perfect reciprocity and correctly identifies an x-default version. Use `generate_html_tags` to inject tags into your ``, `generate_sitemap_entries` for your XML sitemaps, and `validate_hreflang_integrity` to audit your existing implementation for broken links or missing language pairings.


## Available Tools (3)
- **generate_html_tags**: Generates HTML <link> tags for hreflang implementation
- **generate_sitemap_entries**: Generates XML snippet entries for an SEO sitemap
- **validate_hreflang_integrity**: Performs an audit of hreflang implementation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hreflang Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate HTML tags for these URLs: https://mysite.com/en, https://mysite.com/es, with https://mysite.com/en as x-default."

**🤖 AI Agent:**
> <link rel="alternate" hreflang="en" href="https://mysite.com/en" />
<link rel="alternate" hreflang="es" href="https://mysite.com/es" />
<link rel="alternate" hreflang="x-default" href="https://mysite.com/en" />

---

**👤 You:**
> "Check if this URL set is valid: [{targetUrl: 'https://site.com/us', languageCode: 'en', regionCode: 'US'}, {targetUrl: 'https://site.com/uk', languageCode: 'en', regionCode: 'GB'}], default: 'https://site.com/us'"

**🤖 AI Agent:**
> {"isCompliant": true, "missingXDefault": [], "brokenReciprocity": [], "languageGaps": []}

---

**👤 You:**
> "Create sitemap entries for https://mysite.com/fr and https://mysite.com/en, using https://mysite.com/en as x-default."

**🤖 AI Agent:**
> <url><loc>https://mysite.com/fr</loc><xhtml:link rel="alternate" hreflang="en" href="https://mysite.com/en"/><xhtml:link rel="alternate" hreflang="x-default" href="https://mysite.com/en"/></url>
<url><loc>https://mysite.com/en</loc><xhtml:link rel="alternate" hreflang="fr" href="https://mysite.com/fr"/><xhtml:link rel="alternate" hreflang="x-default" href="https://mysite.com/en"/></url>


## ❓ FAQ

**Q: How do I ensure my hreflang tags are valid?**
You can use the `validate_hreflang_integrity` tool to audit your URL list. It checks for reciprocity, x-default presence, and language gaps.

**Q: Can I generate XML sitemap entries?**
Yes, the `generate_sitemap_entries` tool creates the necessary `<url>` and `<xhtml:link>` blocks for your XML sitemaps.

**Q: What is the x-default URL?**
The x-default URL is the fallback version of your page used when no specific language or region matches a user's preference.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hreflang-generator](https://vinkius.com/mcp/hreflang-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hreflang Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hreflang-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hreflang Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hreflang-generator": {
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
