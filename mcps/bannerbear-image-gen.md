# Bannerbear (Image Gen) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bannerbear-image-gen)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bannerbear-image-gen-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bannerbear-image-gen-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate image and video generation via Bannerbear — create dynamic assets from templates and manage collections directly from your AI agent.

## Description
Connect your **Bannerbear** account to any AI agent and automate your design and marketing workflows through natural conversation.

### What you can do

- **Template Management** — List all available templates in your project and fetch detailed layer information using `list_templates` and `get_template`.
- **Dynamic Image Generation** — Create new images by applying text, color, or image modifications to templates with `create_image`.
- **Video Creation** — Generate videos based on video templates and input data frames using `create_video`.
- **Bulk Collections** — Process multiple images at once for high-volume workflows using the `create_collection` action.
- **Asset Retrieval** — Fetch the status and final URLs of your generated images using `get_image` to ensure they are ready for use.

### How it works

1. Subscribe to this server
2. Enter your Bannerbear API Key
3. Start generating visual content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — instantly generate social media banners, ad variations, and personalized content without opening a design tool.
- **Developers** — automate dynamic OG images or PDF generation directly from the code editor or terminal.
- **Content Creators** — quickly produce thumbnails and headers by simply describing the text and template you want to use.


## Available Tools
- **create_collection**: Create multiple images at once as a collection
- **create_image**: Create an image based on a template
- **create_video**: Create a video based on a video template
- **get_image**: Retrieve the details of a previously created image
- **get_template**: Retrieve the details of a specific template
- **list_templates**: Retrieve a list of templates in your project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bannerbear (Image Gen)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Bannerbear templates."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 available: 'Promo Banner' (UID: abc-123), 'Twitter Post' (UID: def-456), and 'Product Card' (UID: ghi-789). Which one would you like to use?

---

**👤 You:**
> "Create an image using template abc-123 with the text 'Summer Sale' in the title layer."

**🤖 AI Agent:**
> I've initiated the image generation for template 'abc-123' with your modifications. The image UID is 'img-xyz-789'. You can check its status in a few moments.

---

**👤 You:**
> "Get the details and URL for image UID img-xyz-789."

**🤖 AI Agent:**
> The image is ready! You can view or download it here: https://bannerbear.com/outputs/img-xyz-789.png. The status is 'completed'.


## Installation & Usage

To install and use the **Bannerbear (Image Gen)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bannerbear-image-gen](https://vinkius.com/mcp/bannerbear-image-gen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
