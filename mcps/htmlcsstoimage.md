# HTMLCSSToImage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/htmlcsstoimage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/htmlcsstoimage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/htmlcsstoimage-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate high-quality images and PDFs from HTML/CSS or URLs directly from your AI agent.

## Description
Connect **HTMLCSSToImage** to your AI agent to automate visual content creation. Convert code snippets or live websites into PNG, JPG, WebP, or PDF files using a simple and powerful API.

### What you can do

- **HTML to Image** — Render custom HTML and CSS snippets into pixel-perfect images instantly.
- **URL Screenshots** — Capture full-page or element-specific screenshots from any public URL with browser-grade precision.
- **Template Management** — Create, edit, and use reusable templates to generate dynamic images with variable data.
- **Batch Processing** — Generate or delete up to 25 images in a single request for high-volume automated workflows.
- **Advanced Customization** — Control viewports, device scaling, Google Fonts, dark mode, and specific CSS selectors for cropping.

### How it works

1. Subscribe to this server
2. Enter your HCTI User ID and API Key
3. Start generating visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate the creation of social sharing images (Open Graph), dynamic reports, or UI mockups.
- **Marketers** — Generate personalized banners, email visuals, and promotional content at scale.
- **Content Creators** — Turn code snippets or web data into shareable visual assets without leaving your chat interface.


## Available Tools
- **batch_create_images**: Create up to 25 images in one request
- **batch_delete_images**: Delete multiple images at once
- **create_image_from_template**: Create an image from a template
- **create_image**: Either html or url is required.

Create an image from HTML/CSS or a URL
- **create_template**: Create a reusable image template
- **delete_image**: Permanently remove an image
- **edit_template**: Edit an existing image template
- **get_image**: Can apply cropping and resizing via query parameters.

Retrieve a generated image file or its metadata
- **get_usage**: Check account usage
- **list_images**: List generated images


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTMLCSSToImage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a PNG image from this HTML: <h1 style='color: blue;'>Hello MCP</h1>"

**🤖 AI Agent:**
> I've generated your image. You can view it here: https://hcti.io/v1/image/example_id.png

---

**👤 You:**
> "Take a full-page screenshot of https://github.com/trending"

**🤖 AI Agent:**
> Capturing the full page... Done! Here is the link to your screenshot of GitHub Trending.

---

**👤 You:**
> "Show me my current API usage for HTMLCSSToImage."

**🤖 AI Agent:**
> You have used 150 out of 1000 images this month. Your account is in good standing.


## Installation & Usage

To install and use the **HTMLCSSToImage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/htmlcsstoimage](https://vinkius.com/mcp/htmlcsstoimage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
