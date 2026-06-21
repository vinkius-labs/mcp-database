# Lorem Picsum MCP Server

Generate placeholder images and retrieve image metadata directly from your AI agent using the Lorem Picsum API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lorem-picsum)

## Overview
**Category:** developer-tools
**Tools Count:** 6

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


## Installation & Usage

To install and use the **Lorem Picsum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lorem-picsum](https://vinkius.com/mcp/lorem-picsum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
