# WordPress Media Uploader MCP Server

This MCP does exactly one thing: it downloads images from a URL and uploads them directly to your WordPress Media Library. Incredible for giving Claude the ability to generate and deploy blog cover images instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-media-uploader)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **WordPress Media Uploader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-media-uploader](https://vinkius.com/mcp/wordpress-media-uploader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
