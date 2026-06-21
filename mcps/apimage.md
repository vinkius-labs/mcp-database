# APImage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apimage)
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


## ❓ FAQ

**Q: Which AI image models are available?**
Use the `list_models` tool to see all supported models. Current options include Flux 1 Dev, Flux 1 Schnell, Stable Diffusion XL, and DALL-E 3. Each model has different strengths for various visual styles.

**Q: Can my AI upscale an image and remove its background in one session?**
Yes. Use `upscale_image` first to increase resolution, then `remove_background` on the result. Both tools accept image URLs, so you can chain operations seamlessly.

**Q: How does inpainting work?**
The `inpaint_image` tool requires three inputs: the source image URL, a mask image URL (white areas = regions to fill), and a text prompt describing what to generate in those areas. The AI fills the masked regions while preserving the rest of the image.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apimage](https://vinkius.com/mcp/apimage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **APImage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apimage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **APImage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apimage": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
