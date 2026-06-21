# Midjourney MCP Server

AI image generation — create, upscale, vary, and blend images using Midjourney's Imagine API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/midjourney)

## Overview
**Category:** ai-frontier
**Tools Count:** 9

## Description
Connect **Midjourney** image generation to any AI agent and create stunning visuals through natural conversation. Generate images from text prompts, upscale to high resolution, create variations, blend images, and even reverse-engineer prompts from existing images.

### What you can do
- **Text-to-Image** — Generate high-quality images from descriptive prompts
- **Upscale** — Enhance any of the 4 grid images to full resolution
- **Variations** — Explore creative alternatives based on any generated image
- **Blend** — Combine 2-5 images into a new composition
- **Describe** — Reverse-engineer a prompt from any image
- **Inpaint** — Edit specific regions of images with masks
- **Task Monitoring** — Track generation progress and retrieve completed images

### How it works
1. Subscribe to this server
2. Enter your Midjourney API key (via Ace Data Cloud)
3. Start generating images from Claude, Cursor, or any MCP client

### Who is this for?
- **Designers** — Rapidly prototype visual concepts and explore variations
- **Content Creators** — Generate custom images for social media, blogs, and presentations
- **Developers** — Integrate AI image generation into apps and workflows


## Available Tools
- **blend**: Provide URLs of existing images to blend together. Optionally add a text prompt to guide the blend.

Blend multiple images together into one composition
- **describe**: Useful for understanding how to recreate styles and compositions.

Generate a text prompt from an image (reverse engineer)
- **get_task_status**: Returns progress percentage, image URLs when ready, and available actions (upscale/variation).

Check the status of an image generation task
- **get_tasks**: Useful for monitoring ongoing generations and finding image IDs for upscale/variation.

List recent image generation tasks
- **imagine**: The prompt should be in English and can include style modifiers like "--ar 16:9" for aspect ratio, "--v 6" for version, "--s" for stylization. Returns a task ID and thumbnail URL. Use the task ID to check generation progress.

Generate an image from text prompt using Midjourney
- **inpaint**: The rest of the image remains unchanged.

Edit a specific region of a generated image using a mask
- **reroll**: Useful when none of the initial 4 images are satisfactory.

Regenerate 4 new images with the same prompt
- **upscale**: Returns the upscaled image URL.

Upscale one of the 4 generated images to higher resolution
- **variation**: Useful for exploring different interpretations of a concept.

Create a variation of one of the 4 generated images


## Installation & Usage

To install and use the **Midjourney** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/midjourney](https://vinkius.com/mcp/midjourney)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
