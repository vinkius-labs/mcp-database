# Kling AI (Generative Video & Image) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kling-ai-generative-video-image)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate cinematic videos and images via Kling AI — use text-to-video, image-to-video, and AI virtual try-on.

## Description
Connect your **Kling AI** account to any AI agent and take full control of state-of-the-art generative video and creative media production through natural conversation.

### What you can do

- **Text-to-Video** — Generate cinematic, high-fidelity AI videos from scenic descriptions using the Kling V3 engine directly from your agent
- **Image Animation** — Transform static frames into dynamic videos (image-to-video) with precise control over motion trajectories and dynamics
- **AI Virtual Try-On** — Map digital garments naturally onto human models using Kolors AI to visualize fashion assets in real-world contexts
- **Lip-Sync Video** — Synchronize speech and mouth movements to video portraits using audio files for professional AI-driven avatars
- **High-Quality Text-to-Image** — Generate up to 4 high-fidelity images simultaneously using the Kolors architecture for rapid visual iteration
- **Task Orchestration** — Manage asynchronous generation jobs, poll for status updates, and retrieve final MP4 and image URLs securely

### How it works

1. Subscribe to this server
2. Enter your Kling Access Key and Secret Key
3. Start generating cinematic media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Editors & Creators** — generate B-roll and cinematic sequences through natural conversation without manual rendering software
- **Creative Directors** — iterate on visual concepts and storyboards rapidly by commanding your agent to generate varied image and video styles
- **E-commerce Teams** — use AI virtual try-on to visualize new garment collections on different human models efficiently


## Available Tools (10)
- **text_to_video**: Returns a Task ID that must be polled until completion (status: succeed). Models: kling-v1, kling-v2, kling-v3.

Generate a cinematic AI video from a text prompt using Kling V3
- **image_to_video**: Returns a Task ID for polling.

Animate a static image into a video using Kling AI
- **get_video_task**: If succeeded, returns the final MP4 URLs.

Check the processing status and retrieve results of a Kling video task
- **list_video_tasks**: List recent Kling AI video generation tasks
- **text_to_image**: Generates up to 4 images. Returns a Task ID for polling.

Generate images from text using Kolors AI model via Kling
- **get_image_task**: When status is succeed, returns the generated image URLs.

Check the processing status of a Kling image task
- **virtual_try_on**: Blends a source garment image naturally onto a target person's photo. Returns a Task ID.

Map digital garments onto human models using AI Virtual Try-On
- **get_tryon_task**: Once succeeded, retrieves the final composited image URL.

Check the status of an AI Virtual Try-On task
- **lip_sync_video**: Returns a Task ID.

Drive mouth movements and synchronize speech to a video portrait
- **get_lipsync_task**: Retrieve the final MP4 when succeed.

Check the status of an AI Lip-Sync task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kling AI (Generative Video & Image)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 5-second cinematic video of a futuristic city in the rain using Kling V3"

**🤖 AI Agent:**
> Video generation task submitted to Kling V3. Task ID: 'vid-98765'. I'm monitoring the render status for you. High-fidelity motion and lighting effects are being computed. I'll provide the MP4 link as soon as it's ready.

---

**👤 You:**
> "Animate this static image into a video with gentle camera pan: [url]"

**🤖 AI Agent:**
> Image-to-video task started. I've set the motion trajectory for a gentle horizontal pan. This will bring your static frame to life with consistent AI-generated dynamics. Your Task ID is 'ani-12345'.

---

**👤 You:**
> "What is the status of my virtual try-on task ID 'try-456'?"

**🤖 AI Agent:**
> Your virtual try-on task 'try-456' has SUCCEEDED. The digital garment has been naturally blended onto the model. You can view and download the final high-resolution composite here: [image-url].


## ❓ FAQ

**Q: Can I check the progress of my video generation task?**
Yes. Use the `get_video_task` tool with your Task ID. Your agent will poll the Kling API and report the current status (Submitted, Processing, or Succeed). Once finished, it will provide the direct MP4 download URLs.

**Q: How does the AI Virtual Try-On work through my agent?**
Use the `virtual_try_on` tool and provide a public URL of a target person and a garment image. Your agent will submit the job to Kolors AI, which naturally blends the clothing onto the person. You can then retrieve the final image using the Task ID.

**Q: Can I synchronize audio to a video portrait using my agent?**
Absolutely. The `lip_sync_video` tool allows you to submit a portrait video and a driving audio file. Your agent will trigger the AI lip-sync process to align the mouth movements to the speech, perfect for creating professional avatars.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kling-ai-generative-video-image](https://vinkius.com/mcp/kling-ai-generative-video-image)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kling AI (Generative Video & Image)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kling-ai-generative-video-image` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kling AI (Generative Video & Image)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kling-ai-generative-video-image": {
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
