# Midjourney MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/midjourney)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI image generation — create, upscale, vary, and blend images using Midjourney's Imagine API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Midjourney** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a cyberpunk city at sunset, 16:9 aspect ratio."

**🤖 AI Agent:**
> 🎨 Image generation started! Task ID: mj_abc123. Check progress with get_task_status. Typical generation time: 30-60 seconds.

---

**👤 You:**
> "Upscale image position 2 from the last generation."

**🤖 AI Agent:**
> 🔍 Image upscaled successfully! Full resolution image URL: https://cdn.midjourney.com/... You can now download or share this image.

---

**👤 You:**
> "Describe this image and tell me what prompt would create it: https://example.com/art.jpg"

**🤖 AI Agent:**
> 📝 Generated prompt: 'ethereal watercolor painting of a lone wolf howling at a blood moon, dark forest silhouette, mystical atmosphere --ar 16:9 --v 6'. Use this prompt with imagine to recreate a similar image.


## ❓ FAQ

**Q: How do I get a Midjourney API key?**
Sign up at [Ace Data Cloud](https://acedata.cloud/) and subscribe to the Midjourney Imagine API service. You'll receive an API key that works with this MCP server.

**Q: What's the difference between upscale and variation?**
Upscale increases resolution of a specific grid image (1-4) to full quality. Variation creates 4 new creative alternatives based on that image's style and composition. Use upscale for final output, variation for exploration.

**Q: How long does image generation take?**
Typically 30-60 seconds. Use get_task_status to check progress. The API returns a task ID immediately, and you can poll for completion or set a callback URL for async notification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/midjourney](https://vinkius.com/mcp/midjourney)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Midjourney** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `midjourney` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Midjourney** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "midjourney": {
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
