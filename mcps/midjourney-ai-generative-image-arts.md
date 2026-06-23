# Midjourney AI (Generative Image Arts) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/midjourney-ai-generative-image-arts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Generate professional AI art via Midjourney — use 'imagine' for text-to-image, upscale grids, and perform camera edits.

## Description
Connect your **Midjourney** account to any AI agent and take full control of state-of-the-art generative art production and professional creative tools through natural conversation.

### What you can do

- **Cinematic Imagine** — Generate high-fidelity AI images from scenic descriptions using Midjourney's latest generative models directly from your agent
- **Precision Upscaling** — Extract and upscale specific tiles from your 2x2 generation grids to retrieve high-resolution final renders securely
- **Visual Variation** — Create brand new structural branches from existing grid images to iterate on visual concepts and aesthetic directions
- **Camera Control (Pan & Zoom)** — Direct your AI shots with specific directional movements (up, down, left, right) or widen perspective using dynamic zoom out levels
- **Image Description** — Reverse engineer prompts from any public image URL, retrieving 4 candidate text descriptions to understand visual concepts natively
- **Multi-Image Blending** — Merge between 2 and 5 source images into a single unique composition, bridging distinct artistic styles flawlessly
- **Task Orchestration** — Manage asynchronous generation jobs, poll for status updates (pending, completed), and monitor your account's job history in real-time

### How it works

1. Subscribe to this server
2. Enter your Midjourney API Key
3. Start generating world-class art from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Artists & Designers** — rapid-prototype visual concepts and aesthetic directions through natural conversation without manual prompt entry
- **Creative Directors** — generate high-quality moodboards and storyboard frames by commanding your agent to iterate on variations and blends
- **Marketing Teams** — produce photorealistic assets and cinematic backgrounds directly from your workspace terminal for high-speed design workflows


## Available Tools (10)
- **generate_image**: Always retrieve the returning Job ID to poll `get_job` tracking its process till completion.

Generate images from a text prompt using Midjourney generative models
- **get_job**: DO NOT loop aggressively, sleep in between.

Get the active execution status of an ongoing Midjourney job
- **list_jobs**: List recent history representing previously executed Midjourney prompts
- **describe_image**: Reverse engineer text descriptions from an input image via Midjourney
- **blend_images**: Pass absolute valid URLs delimited strictly by commas.

Blend 2-5 explicit images into a new unique composition
- **upscale_image**: Polled async.

Extract and upscale a single specific tile off a 2x2 grid
- **generate_variation**: Returns a new Job.

Create variant branches from a specific Midjourney grid image
- **reroll_job**: Re-run identical prompt arguments dropping new sets of outputs
- **pan_image**: Extrapolate frame borders panning natively over a direction
- **zoom_out_image**: Widen the perspective zooming out explicitly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Midjourney AI (Generative Image Arts)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a futuristic cyberpunk city at sunset with neon reflections in 16:9"

**🤖 AI Agent:**
> Generating image… I've triggered the Midjourney imagine task with your prompt and a 16:9 aspect ratio. Your Job ID is 'mj-98765'. I'm monitoring the process. High-fidelity textures and lighting are being computed. I'll provide the 2x2 grid URL as soon as it's ready.

---

**👤 You:**
> "Upscale the first image from grid ID 'mj-98765'"

**🤖 AI Agent:**
> Upscaling tile 1… I've triggered the high-resolution render for your first choice. This will isolate the image and apply advanced AI detail enhancement. I'll provide the final high-res URL once the upscale job completes.

---

**👤 You:**
> "Describe the contents of this image: [url]"

**🤖 AI Agent:**
> Analyzing visual concepts… I've retrieved 4 candidate prompts from Midjourney: 1) 'Minimalist architectural sketch in charcoal', 2) 'Brutalist concrete building perspective', 3) 'Abstract geometric shadows on stone', and 4) 'Architectural blueprint style'. Would you like to use any of these to generate a new variation?


## ❓ FAQ

**Q: How do I check if my Midjourney image is ready?**
Use the `get_job` tool with the Job ID provided. Your agent will poll the API and report the current state (pending or completed). Once finished, it will return the final image URL or the 2x2 grid depending on your task.

**Q: Can I edit an image by zooming out or panning the camera through the agent?**
Absolutely. Use the `pan_image` and `zoom_out_image` tools with a completed Job ID. Your agent will command Midjourney to expand the canvas or shift the focus in your specified direction, creating professional cinematographic edits.

**Q: What does the 'describe' tool do?**
The `describe_image` tool reverse engineers prompts. Provide an image URL, and your agent will retrieve 4 candidate text descriptions from Midjourney, showing you the exact words and styles used to create that visual concept.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/midjourney-ai-generative-image-arts](https://vinkius.com/mcp/midjourney-ai-generative-image-arts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Midjourney AI (Generative Image Arts)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `midjourney-ai-generative-image-arts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Midjourney AI (Generative Image Arts)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "midjourney-ai-generative-image-arts": {
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
