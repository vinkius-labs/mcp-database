# Playground AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/playground-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate, inpaint, upscale, and transform images using Playground AI's powerful models via natural language.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Playground AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 1024x1024 image of a cyberpunk coffee cup in neon lighting."

**🤖 AI Agent:**
> Payload dispatched holding spatial constraints to 1024x1024 pixels. Using default Model 'Playground v3'. The system returns generation block `ID: 9x8A-CUP`. The finalized render URL is ready: [View Graphic]. Want to apply an iterative 2x Upscale on it now?

---

**👤 You:**
> "Upscale this image to 4x its size `https://example.com/small_icon.png`."

**🤖 AI Agent:**
> Upscaling protocol engaged. Submitted target to `upscale_image` invoking factor constraint '4'. The engine interpolated logical pixels correctly matching standard textures natively. Result pointer: [High-Res URL].

---

**👤 You:**
> "Remove the background from the image at `https://example.com/person.jpg`."

**🤖 AI Agent:**
> Background segmentation dispatched via `remove_background`. The deep learning layer masked the subject heavily and omitted out-of-bounds layer fragments. I've received the pristine transparent PNG rendering back. The new asset is currently available at `[Extracted PNG URL]`. Would you like me to map it in a new CSS class?


## ❓ FAQ

**Q: Can my AI automatically remove a background and embed the image into my project?**
Yes! The agent triggers the `remove_background` method on any public image URL. Playground internally isolates the core subject, dropping the background layers, and replies with a secure pointer URL. Your agent can instantly fetch the response string and code an `<img>` tag placing the clean asset directly into the UI mapping you're developing.

**Q: How exactly does `outpaint_image` expand the canvas?**
The tool passes the target image alongside the literal specific expansion vectors ('up', 'down', 'left', 'right') and a guiding context text. The diffusion nodes generate purely new mathematical tensor states radiating outward, predicting the lighting, shadows, and environment strictly following your prompt rules without stretching existing pixels.

**Q: Can I enforce specific structural references using ControlNet constraints?**
Yes. Instead of standard generation, invoke `generate_with_controlnet`. You upload a scribble or an edges-only mapping layout as your source. By defining the explicit type ('canny', 'depth', 'pose', 'scribble'), the AI strictly anchors its conceptual render to those physical guiding constraints rather than randomizing spatial architecture.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/playground-ai](https://vinkius.com/mcp/playground-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Playground AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `playground-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Playground AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "playground-ai": {
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
