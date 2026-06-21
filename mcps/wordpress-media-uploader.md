# WordPress Media Uploader MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-media-uploader)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wordpress-media-uploader-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wordpress-media-uploader-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

This MCP does exactly one thing: it downloads images from a URL and uploads them directly to your WordPress Media Library. Incredible for giving Claude the ability to generate and deploy blog cover images instantly.

## Description
We refused to build a bloated WordPress integration that gives an AI agent terrifying access to delete your pages, read your entire database, or install plugins. Instead, this MCP server provides a surgical, zero-trust bridge: **just uploading images to your Media Library.**

Your AI agent gains the immediate ability to act as a complete content production agency. It can generate an article, use a tool like DALL-E or Midjourney to generate a cover image, and then use this tool to seamlessly upload that image directly into your WordPress site.

### The Superpowers

- **Zero-Friction Asset Management:** End the 'download-upload' nightmare. The AI fetches the image from a URL and drops it into your CMS automatically.
- **Zero-Bloat Integration:** No custom plugins required. It uses the native WordPress REST API `/wp-json/wp/v2/media`. You only need an Application Password (a native WordPress feature).
- **Absolute Containment:** Because this is strictly a "Push-only" creation tool scoped only to Media, the agent is physically incapable of publishing text content, deleting plugins, or reading customer data. It is a completely secure, one-way funnel.


## Available Tools
- **upload_wordpress_media**: Provide the public sourceUrl, a descriptive filename (like "seo-cover-image.jpg"), and an optional alt text for SEO.

Downloads an image from a public URL and uploads it to the WordPress Media Library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress Media Uploader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here is an image URL: https://example.com/generated-cover.png. Upload it to my WordPress as 'seo-future-ai-cover.png' with the alt text 'The Future of AI'."

**🤖 AI Agent:**
> The image was uploaded successfully! Here is the public URL on your site: https://myblog.com/wp-content/uploads/2026/05/seo-future-ai-cover.png


## Installation & Usage

To install and use the **WordPress Media Uploader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-media-uploader](https://vinkius.com/mcp/wordpress-media-uploader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
