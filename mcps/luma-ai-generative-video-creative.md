# Luma AI (Generative Video & Creative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/luma-ai-generative-video-creative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate cinematic AI videos and images via Luma — use Dream Machine for text-to-video, image-to-video, and professional camera control.

## Description
Connect your **Luma AI** account to any AI agent and take full control of state-of-the-art generative video production and professional creative tools through natural conversation.

### What you can do

- **Cinematic Text-to-Video** — Generate high-fidelity AI videos from scenic descriptions using Luma Dream Machine (Ray-2 model) directly from your agent
- **Image Animation** — Transform static frames into dynamic videos (image-to-video) with industry-leading motion coherence and photorealism
- **Professional Camera Control** — Direct your AI shots with specific movements including pan, tilt, dolly, and orbit using structured movement parameters
- **Video Extension & Looping** — Seamlessly continue existing scenes with additional footage or create perfect looping videos for social media and backgrounds
- **Keyframe Interpolation** — Create smooth, high-quality video transitions between two distinct keyframe images to bridge visual concepts effectively
- **Photorealistic Text-to-Image** — Generate stunning high-resolution images using the Luma Photon-1 model for rapid visual iteration and design
- **Task Orchestration** — Manage asynchronous generation jobs, poll for status updates (queued, dreaming, completed), and monitor your API credit balance securely

### How it works

1. Subscribe to this server
2. Enter your Luma AI API Key
3. Start generating cinematic media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Editors & Creators** — generate high-quality B-roll and cinematic sequences through natural conversation without manual rendering
- **Creative Directors** — rapid-prototype visual concepts and storyboards by commanding your agent to generate varied styles and camera paths
- **AI Artists & Designers** — iterate on photorealistic imagery and complex video transitions directly from your workspace


## Available Tools
- **lm.get_generation**: Get the status and result of a Luma Dream Machine generation. Returns state (queued/dreaming/completed/failed) and video URL
- **lm.list_generations**: List recent Luma Dream Machine generations. Returns generation IDs, prompts, states, and timestamps
- **lm.delete_generation**: Delete a Luma Dream Machine generation and its video
- **lm.extend_video**: Extend an existing Luma video with additional footage. Seamlessly continues the scene
- **lm.interpolate**: Create smooth video transition between two keyframe images using Luma Dream Machine
- **lm.camera_control**: Generate video with specific camera movements using Luma Dream Machine. Supports pan, tilt, dolly, orbit
- **lm.text_to_image**: Generate photorealistic images using Luma Photon-1 model
- **lm.get_credits**: Get current Luma Dream Machine credit balance
- **lm.text_to_video**: ), and loop (true/false). Poll get_generation for results.

Generate cinematic AI video from a text prompt using Luma Dream Machine (Ray-2 model). Industry-leading motion coherence and photorealism
- **lm.image_to_video**: Animate a still image into video using Luma Dream Machine. Image becomes the first frame


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Luma AI (Generative Video & Creative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 5-second cinematic video of a futuristic spaceship landing on a neon planet"

**🤖 AI Agent:**
> Generating cinematic video… I've triggered Luma Dream Machine with your prompt. Your Generation ID is 'gen-98765'. I'm monitoring the status. High-fidelity motion and lighting are being computed. I'll provide the MP4 link as soon as it's ready.

---

**👤 You:**
> "Animate this static image into a video: [url]"

**🤖 AI Agent:**
> Image-to-video task started. I'm using your image as the source frame for Luma Dream Machine. This will bring your static visual to life with consistent AI dynamics. Your Generation ID is 'gen-12345'.

---

**👤 You:**
> "Show me my last 3 Luma generations"

**🤖 AI Agent:**
> I've retrieved your recent generations: 1) 'Spaceship Landing' (Status: Completed), 2) 'Neon Forest' (Status: Dreaming), and 3) 'Abstract Waves' (Status: Completed). Would you like to see the video links for the completed ones?


## ❓ FAQ

**Q: How do I check if my video generation is finished?**
Use the `lm.get_generation` tool with the Generation ID provided. Your agent will poll the Luma API and report the current state (queued, dreaming, or completed). Once finished, it will return the final MP4 video URL.

**Q: Can I control the camera movement in my AI-generated video?**
Absolutely. Use the `lm.camera_control` tool. You can provide a scene prompt and a JSON block defining the movement type (e.g., orbit, pan, tilt) and magnitude, allowing for professional cinematographic directing.

**Q: Can my agent extend an existing Luma video with more footage?**
Yes. The `lm.extend_video` tool allows you to provide a continuation prompt and a previous Generation ID. Your agent will trigger Luma to seamlessly expand the scene, maintaining visual and structural consistency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/luma-ai-generative-video-creative](https://vinkius.com/mcp/luma-ai-generative-video-creative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Luma AI (Generative Video & Creative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `luma-ai-generative-video-creative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Luma AI (Generative Video & Creative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "luma-ai-generative-video-creative": {
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
