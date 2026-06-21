# Stability AI MCP Server

Connect your AI to Stability AI's powerful image generation models. Create, upscale, and edit high-quality images directly and efficiently.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stability-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Integrate the industry-leading generative visual capabilities of **Stability AI** seamlessly into your conversational LLM workflows. Empower your creative and design teams to rapidly generate photorealistic drafts, upscale low-resolution assets, or systematically remove backgrounds from product photography without relying on external design software. Connect your API securely to your local configuration, interact naturally via conversation to iterate on images, and streamline your entire design pipeline effortlessly.

### What you can do

- **Core Image Generation** — Synthesize net-new images from detailed text prompts and visual parameters invoking `generate_image`, utilizing state-of-the-art diffusion models.
- **Image Upscaling & Enhancement** — Resolve low-resolution graphics mathematically, increasing dimensions while retaining structural fidelity using `upscale_image`.
- **Precision Editing** — Eradicate complex subject backgrounds instantly from product portraits securely and cleanly invoking `remove_background`.
- **Inpainting & Masking** — Surgically replace isolated regions within a graphic layout, maintaining exact consistency mathematically utilizing `inpaint_image`.

### How it works

1. Establish the Stability AI MCP connector reliably on your active AI system.
2. In the MCP settings, securely attach your official API Key, effectively binding operations locally.
3. Prompt your agent objectively: "Generate a 1024x1024 photorealistic mockup focusing on a modern smart home device, then cleanly remove the background."

### Who is this for?

- **Digital Marketing Agencies** — Automate iterative campaign graphic creation rapidly, testing diverse ad variations procedurally directly via the terminal.
- **E-Commerce Managers** — Sanitize product photography backgrounds systematically, standardizing catalog appearances objectively in bulk.
- **Creative Operations Leaders** — Expedite concept-art workflows seamlessly converting initial rough sketches to high-resolution presentations for stakeholders.


## Available Tools
- **generate_core_v2**: Optimized for speed and quality.

Generate an image using the Stable Image Core model
- **generate_sd35**: Choose from "sd3.5-large", "sd3.5-large-turbo", or "sd3.5-medium".

Generate an image using Stable Diffusion 3.5
- **generate_ultra_v2**: Best for final production assets.

Generate a high-end photorealistic image
- **get_credit_balance**: Retrieves your current Stability AI credit balance
- **image_to_image_v1**: Requires engine_id and prompt.

Transform an existing image based on a text prompt
- **inpaint_image**: Edits specific regions of an image based on a prompt
- **list_engines**: These IDs are required for v1 generation tools.

List all available image generation engines on Stability AI
- **remove_background**: Removes the background from an image
- **text_to_image_v1**: Provide engine_id, prompt, width, and height. Width/Height must be multiples of 64.

Generate an image from a text prompt using v1 engines
- **upscale_image**: Provide a guidance prompt to help the model maintain quality.

Increases image resolution while preserving detail


## Installation & Usage

To install and use the **Stability AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stability-ai](https://vinkius.com/mcp/stability-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
