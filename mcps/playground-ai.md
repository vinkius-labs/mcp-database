# Playground AI MCP Server

Generate, inpaint, upscale, and transform images using Playground AI's powerful models via natural language.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/playground-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Connect your AI agent directly to the **Playground AI** compute clusters. Eliminate manual interface dragging by instructing your LLM (Claude, Cursor) to natively generate, radically outpaint, or surgically inpaint high-resolution visual components using the `Playground v3` pipeline.

### What you can do

- **Direct Image Generation** — Generate pristine assets instantly. Use the `generate_image` tool explicitly defining prompt nuances and tensor geometries (like 1024x1024).
- **ControlNet & Transformations** — Substantially alter base images. Tell the agent to use `controlnet` (depth/canny) or apply raw `transform_image` overrides mutating your sketches into polished renders.
- **Precision Editing** — Execute flawless structural edits. Instruct the AI to seamlessly `remove_background` and isolate elements, or use `inpaint_image` overlaying explicit masks.
- **Upscaling & Outpainting** — Scale blurry inputs intelligently up to 4x, or instruct the diffusion model to geometrically expand boundary borders utilizing `outpaint_image`.

### How it works

1. Append the Playground integration strictly to your MCP setup
2. Provide your Playground API Key
3. Start rendering graphics and UI components directly from code comments

### Who is this for?

- **Web Developers** — generate perfectly sized graphical placeholders without opening a visual editor.
- **Concept Artists** — automate repetitive masking and background removal using the agent's `remove_background` node.
- **Creative Directors** — apply instantaneous upscaling or outpainting adjustments natively while discussing the copy.


## Available Tools
- **generate_image**: Triggers immediate billing execution per inference step.

Generate images from a text prompt using Playground AI. Playground offers multiple AI models including Playground v3 and SDXL variants for creative image generation. Instructions: Pass prompt, model name, width, height (multiples of 64)
- **transform_image**: Transform an existing image with a text prompt using Playground AI. Strength controls how much the image changes (0-1). Instructions: Pass prompt, public image URL, and strength
- **inpaint_image**: Inpaint specific areas of an image using Playground AI. Uses a mask to define regions. Instructions: Pass prompt, image URL, and mask image URL (white = edit area)
- **upscale_image**: Upscale an image using Playground AI. Enhances resolution and detail. Instructions: Pass image URL and scale factor (2 or 4)
- **remove_background**: Remove the background from an image using Playground AI. Returns transparent PNG. Instructions: Pass public image URL
- **outpaint_image**: Extend an image beyond its borders using Playground AI. AI generates new content in the specified direction. Instructions: Pass prompt, image URL, direction (up/down/left/right)
- **generate_with_controlnet**: Generate images with ControlNet guidance using Playground AI. Control types: canny, depth, pose, scribble. Instructions: Pass prompt, reference image URL, control type
- **list_models**: List available models on Playground AI. Returns model names, descriptions, and capabilities
- **get_generation**: Get details of a Playground AI generation by ID. Returns images, prompt, model, and metadata
- **list_generations**: List recent generations on Playground AI. Returns generation IDs, prompts, and timestamps


## Installation & Usage

To install and use the **Playground AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playground-ai](https://vinkius.com/mcp/playground-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
