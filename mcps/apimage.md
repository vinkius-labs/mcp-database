# APImage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apimage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apimage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apimage-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search and license editorial photography from one of the world largest press image archives for media and publishing.

## Description
Connect your **APImage** account to any AI agent and manage your entire image generation and editing workflow through natural conversation.

### What you can do

- **Text-to-Image** — Generate images from text descriptions using multiple AI models (Flux, Stable Diffusion, DALL-E)
- **Background Removal** — Remove backgrounds from any image and receive transparent PNGs
- **Prompt Enhancement** — Automatically expand simple prompts into detailed descriptions for better results
- **Image Upscaling** — Increase image resolution by 2x or 4x while preserving quality
- **Image-to-Image** — Transform existing images based on text prompts while keeping general structure
- **Inpainting** — Fill in masked areas of images with AI-generated content based on text prompts
- **Model Selection** — Browse available AI models and choose the best one for each task
- **Generation History** — Review all previously generated images with prompts, parameters, and download URLs

### How it works

1. Subscribe to this server
2. Enter your **API Key** from your APImage account settings
3. Start generating images from Claude, Cursor, or any MCP client

### Who is this for?

- **Designers** — generate concept art and mockups directly from the code editor
- **Marketing Teams** — create campaign visuals and product images on demand
- **Developers** — automate asset creation for apps and websites


## Available Tools
- **check_apimage_status**: Verify API connectivity
- **enhance_prompt**: Enhance a generation prompt
- **generate_image**: Optionally specify the model.

Generate an image from a prompt
- **get_generation**: Get generation details
- **image_to_image**: Transform an image with a prompt
- **inpaint_image**: Inpaint a masked region
- **list_generations**: List generation history
- **list_models**: List available models
- **remove_background**: Remove image background
- **upscale_image**: Upscale an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **APImage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a futuristic city at sunset using the Flux model."

**🤖 AI Agent:**
> Image generated! Here's your futuristic cityscape at sunset using Flux 1 Dev (Generation ID: gen_8291). The image features a skyline with glass towers reflecting orange and purple hues. Would you like to upscale it or generate a variation?

---

**👤 You:**
> "Remove the background from this product photo: https://example.com/product.jpg"

**🤖 AI Agent:**
> Background removed! The product is now on a transparent background (PNG format). Download URL: https://apimage.org/results/bg_removed_4821.png. Would you like to place it on a new background?

---

**👤 You:**
> "Enhance this prompt: 'a cat sitting on a windowsill'."

**🤖 AI Agent:**
> Enhanced prompt: 'A fluffy tabby cat sitting peacefully on a sun-drenched wooden windowsill, warm golden afternoon light streaming through lace curtains, potted herbs in the background, soft bokeh, photorealistic, 4K detail'. Would you like to generate an image with this enhanced prompt?


## Installation & Usage

To install and use the **APImage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apimage](https://vinkius.com/mcp/apimage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
