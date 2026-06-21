# Image Router MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/image-router)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Route image generation requests to the best AI model automatically based on prompt type, style, and quality requirements.

## Description
Connect your **ImageRouter** account to any AI agent and manage AI image generation.

### What you can do

- **Image Generation** — Create images from text prompts with any supported model
- **Advanced Generation** — Full control over size, steps, seed, and negative prompts
- **Image Editing** — Modify existing images based on text descriptions
- **Model Library** — Browse and filter models by category
- **Style Presets** — Apply artistic styles to generations
- **Upscaling** — Increase image resolution
- **Variations** — Create visual variations of existing images
- **Task Status** — Check async generation progress


## Available Tools
- **check_imagerouter_status**: Verify API connectivity
- **edit_image**: Edit an existing image
- **generate_image_advanced**: Generate with full options
- **generate_image**: Generate an image from text
- **generate_variation**: Generate image variation
- **get_model**: Get model details
- **get_generation_status**: Check generation status
- **list_models_by_category**: List models by category
- **list_models**: List available models
- **list_styles**: List image styles
- **upscale_image**: Upscale an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Image Router** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a futuristic city at sunset."

**🤖 AI Agent:**
> Image generated! 1024x1024 using Stable Diffusion XL. The scene shows towering glass buildings with warm golden light reflecting off surfaces.

---

**👤 You:**
> "List all available image models."

**🤖 AI Agent:**
> 18 models available: Stable Diffusion XL, DALL-E 3, Playground v2.5, DreamShaper XL, and 14 more. Filter by category for specific styles.

---

**👤 You:**
> "Upscale this image to 2x resolution."

**🤖 AI Agent:**
> Image upscaled from 512x512 to 1024x1024. Details enhanced with AI super-resolution.


## ❓ FAQ

**Q: Can my AI generate images from text?**
Yes. `generate_image` creates images from any text prompt using AI models like Stable Diffusion.

**Q: Can I upscale or create variations?**
Yes. `upscale_image` increases resolution and `generate_variation` creates visual alternatives of an existing image.

**Q: How do I browse available models?**
Use `list_models` for all models or `list_models_by_category` to filter by style category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/image-router](https://vinkius.com/mcp/image-router)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Image Router** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `image-router` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Image Router** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "image-router": {
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
