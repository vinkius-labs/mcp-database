# Ideogram MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ideogram)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate stunning images from text prompts with an AI model that excels at typography, logos, and photorealistic compositions.

## Description
Connect your **Ideogram** account to any AI agent and create AI-generated images through natural conversation.

### What you can do

- **Text-to-Image** — Generate high-quality images from text prompts with style, aspect ratio, and model controls
- **Image Remix** — Transform existing images with new prompts while preserving composition
- **Image Editing** — Edit specific areas of images with inpainting and masking
- **Upscaling** — Increase image resolution while preserving quality and detail
- **Image Description** — Analyze images and generate detailed text descriptions
- **Gallery** — Browse previously generated images with metadata

### How it works

1. Subscribe to this server
2. Enter your Ideogram API Key from the developer dashboard
3. Start generating images from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers** — generate concept art, mockups, and visual assets through AI
- **Marketers** — create social media graphics, ad creatives, and brand visuals
- **Developers** — integrate AI image generation into workflows


## Available Tools (12)
- **check_ideogram_status**: Verify connectivity
- **get_image**: Get image details
- **list_images**: List images
- **list_models**: List models
- **delete_image**: Delete an image
- **describe_image**: Describe an image
- **edit_image**: Edit an image
- **generate_image**: Generate an image
- **get_account**: Get account info
- **list_styles**: List styles
- **remix_image**: Remix an image
- **upscale_image**: Upscale an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ideogram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a futuristic cityscape at sunset in 16:9 aspect ratio with realistic style."

**🤖 AI Agent:**
> Image generated! Prompt: 'Futuristic cityscape at sunset with neon lights, flying vehicles, and towering skyscrapers reflecting golden light'. Style: Realistic, Aspect: 16:9, Model: v2. Resolution: 1920x1080. Generation time: 8 seconds. The image shows a dramatic skyline with warm sunset tones. Would you like to upscale it, remix it with different colors, or generate variations?

---

**👤 You:**
> "Upscale my last generated image to 4K and describe what it contains."

**🤖 AI Agent:**
> Upscaled! Original: 1920x1080 → 4K: 3840x2160. Quality preserved with enhanced detail in building textures and lighting effects. Description: 'A futuristic metropolis at golden hour featuring towering glass skyscrapers with holographic advertisements, elevated transit lines, flying vehicles against an orange-purple gradient sky, reflective wet streets with neon signage, and lush rooftop gardens on lower buildings.' Would you like to edit specific areas or generate a new image?

---

**👤 You:**
> "Show my recent generated images and remix the best one with a winter theme."

**🤖 AI Agent:**
> Recent images: 8 generated this week. 1) Futuristic cityscape (4K, realistic). 2) Logo design 'TechFlow' (1:1, design). 3) Mountain landscape (16:9, realistic). 4) Product mockup (4:3). Remixing #1 with winter theme... Done! New image: Same cityscape composition but with snow-covered buildings, ice reflections, aurora borealis sky, and frost on windows. Style maintained, season transformed. Would you like to compare or edit?


## ❓ FAQ

**Q: Can I generate images with specific styles and aspect ratios?**
Yes. The `generate_image` tool accepts a text prompt along with style presets (realistic, design, 3D, anime), aspect ratio (1:1, 16:9, 9:16, etc.), and model version. You can control the output precisely for different use cases.

**Q: Can I edit specific parts of an existing image?**
Yes. Use `edit_image` with a source image and mask to modify specific regions using inpainting. Use `remix_image` to transform an image with a new prompt while preserving its overall composition and structure.

**Q: How does Ideogram authentication work?**
Ideogram uses a custom `Api-Key` header (not Bearer). Your API key is generated from the Ideogram developer dashboard and sent in all requests to `api.ideogram.ai`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ideogram](https://vinkius.com/mcp/ideogram)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ideogram** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ideogram` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ideogram** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ideogram": {
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
