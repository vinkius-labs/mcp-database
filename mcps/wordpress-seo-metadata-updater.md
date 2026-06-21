# WordPress SEO Metadata Updater MCP Server

This MCP does exactly one thing: it rewrites the SEO title, meta description, and focus keyword of an existing WordPress post. Works with both Yoast SEO and RankMath automatically. Incredible for turning Claude into an SEO analyst that fixes your blog rankings while you sleep.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-seo-metadata-updater)

## Overview
**Category:** marketing-automation
**Tools Count:** 1

## Description
We refused to build a bloated WordPress integration that gives an AI agent terrifying access to delete your pages, read your entire database, or install plugins. Instead, this MCP server provides a surgical, zero-trust bridge: **just updating the SEO meta fields of a single post.**

Your AI agent gains the immediate ability to act as a senior SEO analyst. Feed it a post ID, and it will craft a perfectly optimized title tag, a high-CTR meta description, and set the focus keyword—all pushed directly into the fields that Yoast SEO or RankMath use to render your `<head>` tags.

### The Superpowers

- **Plugin-Agnostic Magic:** We push meta fields for BOTH Yoast SEO (`_yoast_wpseo_title`) and RankMath (`rank_math_title`) in a single request. The WordPress REST API silently ignores keys that don't belong to the installed plugin. You never need to tell us which one you use.
- **Bulk Optimization Potential:** Combine this with a simple script that lists your post IDs, and the AI can rewrite the SEO metadata of your entire blog archive in a single session.
- **Absolute Containment:** Because this is strictly a metadata-only update tool, the agent cannot modify your post content, cannot delete pages, and cannot read your private drafts. It only touches the SEO fields. A completely secure, surgical operation.


## Available Tools
- **update_wordpress_seo**: Provide the numeric post ID, the optimized SEO title, the compelling meta description, and a focus keyword. Works automatically with both Yoast SEO and RankMath plugins. IMPORTANT: WordPress REST API silently ignores Yoast SEO keys unless the user adds a snippet to their functions.php to register them. If you suspect the update didn't work, tell the user to add the "register_meta" snippet for Yoast.

Updates the SEO metadata (title, description, focus keyword) of an existing WordPress post for Yoast SEO and RankMath


## Installation & Usage

To install and use the **WordPress SEO Metadata Updater** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-seo-metadata-updater](https://vinkius.com/mcp/wordpress-seo-metadata-updater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
