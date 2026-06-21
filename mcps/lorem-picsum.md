# Lorem Picsum MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lorem-picsum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lorem-picsum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lorem-picsum-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate placeholder images and retrieve image metadata directly from your AI agent using the Lorem Picsum API.

## Description
Integrate **Lorem Picsum** into your AI workflows to instantly generate placeholder images, fetch image metadata, and manage visual assets for development and design.

### What you can do

- **Image Discovery** — Use `list_images` to browse available photos with full metadata including authors and original dimensions.
- **Random Generation** — Generate URLs for random images with `get_random_image_url`, customizing width, height, blur, or grayscale effects.
- **Specific Retrieval** — Fetch specific images by ID using `get_specific_image_url` or use `get_seed_image_url` for consistent UI testing.
- **Metadata Inspection** — Retrieve detailed author and format information for any image using `get_image_info` or `get_seed_info`.
- **Format Control** — Choose between JPG and WebP formats and apply Gaussian blur filters directly through tool parameters.

### How it works

1. Subscribe to this server
2. No API key is required for public access
3. Start generating image assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly populate UI mockups with realistic placeholder images without leaving the code editor
- **UI/UX Designers** — test layouts with different image dimensions and effects like blur or grayscale
- **Content Managers** — find high-quality open-source images and their author credits for attribution


## Available Tools
- **get_image_info**: Get metadata for a specific image ID
- **get_random_image_url**: Can be customized with dimensions, grayscale, blur, and file extensions.

Get a random image URL with specified dimensions and options
- **get_seed_image_url**: Get a static random image URL based on a seed string
- **get_seed_info**: Get metadata for a specific image seed
- **get_specific_image_url**: Get a specific image URL by ID with dimensions and options
- **list_images**: Retrieve a paginated list of available images


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lorem Picsum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a random 800x600 image URL with a blur effect of 5."

**🤖 AI Agent:**
> I've generated the URL for you. You can use this 800x600 blurred image: https://picsum.photos/800/600?blur=5

---

**👤 You:**
> "List 5 images from Lorem Picsum and show their authors."

**🤖 AI Agent:**
> I've fetched 5 images for you. Notable ones include Image ID 0 by Alejandro Escamilla and Image ID 1 by Alejandro Escamilla. Would you like the metadata for a specific one?

---

**👤 You:**
> "Get the details for image ID 237."

**🤖 AI Agent:**
> Image ID 237 was captured by André Spieker. Its original dimensions are 3500x2095. You can view it here: https://picsum.photos/id/237/3500/2095


## Installation & Usage

To install and use the **Lorem Picsum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lorem-picsum](https://vinkius.com/mcp/lorem-picsum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
