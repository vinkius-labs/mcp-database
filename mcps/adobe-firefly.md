# Adobe Firefly MCP Server

Generate images and vectors via Adobe Firefly — perform generative fill and expand, create text effects, and remove backgrounds directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/adobe-firefly)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Adobe Firefly** developer account to any AI agent and take full control of your commercially safe generative AI image and vector creation through natural conversation.

### What you can do

- **Text-to-Image Orchestration** — Generate photorealistic or stylized images from text prompts utilizing Firefly's elite model 5 for high-fidelity output natively
- **Generative Fill & Expand** — Fill masked areas or expand images beyond their borders by commanding absolute explicit text payloads to generate surrounding context flawlessly
- **Text-to-Vector Synthesis** — Produce editable SVG vector graphics from descriptive prompts, bringing Adobe Illustrator-grade assets to your AI agent loops
- **Intelligent Image Editing** — Upload source images to perform background removals, generate similar variations, or create object composites synchronously
- **Text Effects & Art** — Transform plain textual strings into stylized visual art by applying AI-generated textures and effects according to style prompts
- **Asset Storage & Management** — Manage uploaded image binaries and retrieve unique IDs to orchestrate complex multi-step generative operations securely
- **Model Discovery** — Enumerate available Firefly models and versions to evaluate capabilities and determine precise active inference boundaries natively

### How it works

1. Subscribe to this server
2. Enter your Adobe Firefly Client ID and Client Secret (found in Adobe Developer Console > Projects > Firefly Services)
3. Start generating AI-powered visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers & Creatives** — generate commercially safe reference images and vectors without switching to Photoshop or Illustrator
- **Marketers** — create stylized text effects and social media visuals using natural language conversation
- **Content Creators** — remove backgrounds and expand image borders to fit different aspect ratios in real-time
- **Developers** — test and debug Firefly API integrations and verify generative fill schemas through natural conversation


## Available Tools
- **text_to_image**: Model 5 offers photorealistic output. Instructions: Pass prompt and count (1-4).

Generate images from a text prompt using Adobe Firefly
- **generative_fill**: Instructions: Upload image first, get image_id and mask_id.

Fill masked areas of an image using Adobe Firefly Generative Fill
- **generative_expand**: Instructions: Pass image_id, target width/height.

Expand an image beyond its borders using Adobe Firefly
- **text_to_vector**: Instructions: Pass a descriptive prompt.

Generate SVG vectors from a text prompt using Adobe Firefly
- **upload_image**: Returns image ID. Instructions: Pass a publicly accessible URL.

Upload an image to Adobe Firefly storage
- **remove_background**: Instructions: Upload image first, pass image_id.

Remove the background from an image using Adobe Firefly
- **generate_similar**: Instructions: Upload reference first, pass image_id and prompt.

Generate images similar to a reference using Adobe Firefly
- **generate_object**: Instructions: Pass descriptive prompt.

Generate an object composite image using Adobe Firefly
- **text_effects**: Instructions: Pass the text and a style prompt.

Apply AI text effects using Adobe Firefly
- **list_models**: List available Firefly models


## Installation & Usage

To install and use the **Adobe Firefly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adobe-firefly](https://vinkius.com/mcp/adobe-firefly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
