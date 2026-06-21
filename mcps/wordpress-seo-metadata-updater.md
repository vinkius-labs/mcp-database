# WordPress SEO Metadata Updater MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-seo-metadata-updater)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

This MCP does exactly one thing: it rewrites the SEO title, meta description, and focus keyword of an existing WordPress post. Works with both Yoast SEO and RankMath automatically. Incredible for turning Claude into an SEO analyst that fixes your blog rankings while you sleep.

## Description
We refused to build a bloated WordPress integration that gives an AI agent terrifying access to delete your pages, read your entire database, or install plugins. Instead, this MCP server provides a surgical, zero-trust bridge: **just updating the SEO meta fields of a single post.**

Your AI agent gains the immediate ability to act as a senior SEO analyst. Feed it a post ID, and it will craft a perfectly optimized title tag, a high-CTR meta description, and set the focus keyword—all pushed directly into the fields that Yoast SEO or RankMath use to render your `<head>` tags.

### The Superpowers

- **Plugin-Agnostic Magic:** We push meta fields for BOTH Yoast SEO (`_yoast_wpseo_title`) and RankMath (`rank_math_title`) in a single request. The WordPress REST API silently ignores keys that don't belong to the installed plugin. You never need to tell us which one you use.
- **Bulk Optimization Potential:** Combine this with a simple script that lists your post IDs, and the AI can rewrite the SEO metadata of your entire blog archive in a single session.
- **Absolute Containment:** Because this is strictly a metadata-only update tool, the agent cannot modify your post content, cannot delete pages, and cannot read your private drafts. It only touches the SEO fields. A completely secure, surgical operation.


## Available Tools (1)
- **update_wordpress_seo**: Provide the numeric post ID, the optimized SEO title, the compelling meta description, and a focus keyword. Works automatically with both Yoast SEO and RankMath plugins. IMPORTANT: WordPress REST API silently ignores Yoast SEO keys unless the user adds a snippet to their functions.php to register them. If you suspect the update didn't work, tell the user to add the "register_meta" snippet for Yoast.

Updates the SEO metadata (title, description, focus keyword) of an existing WordPress post for Yoast SEO and RankMath


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress SEO Metadata Updater** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Optimize the SEO of post #42. The article is about AI automation for small businesses."

**🤖 AI Agent:**
> I've updated the SEO metadata for post #42:
- **Title:** AI Automation for Small Business: The Complete 2026 Guide
- **Description:** Discover how small businesses are using AI automation to cut costs by 40%. Step-by-step guide with real examples. Try for free.
- **Focus Keyword:** AI automation small business


## ❓ FAQ

**Q: Which SEO plugin do I need?**
Either Yoast SEO or RankMath. This MCP sends metadata fields for both plugins simultaneously in every request. WordPress silently ignores the fields that don't belong to your installed plugin, so it 'just works' regardless of which one you chose.

**Q: Can the AI change the content of my blog posts?**
No. This MCP only sends the `meta` payload to the post update endpoint. The actual post `title` and `content` fields are never included in the request body, making it physically impossible for the AI to alter your published text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-seo-metadata-updater](https://vinkius.com/mcp/wordpress-seo-metadata-updater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WordPress SEO Metadata Updater** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wordpress-seo-metadata-updater` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WordPress SEO Metadata Updater** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wordpress-seo-metadata-updater": {
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
