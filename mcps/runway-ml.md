# Runway ML MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-ml)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Empower your AI with Runway ML's advanced video generation capabilities to seamlessly create, animate, and interpolate high-quality clips using Gen-3 and Gen-4 Turbo models directly from chat.

## Description
Connect your AI to **Runway ML**, the pioneer in applied AI research shaping the next era of art, entertainment and human creativity. This powerful integration empowers you to tap directly into Runway's cutting-edge Gen-3 Alpha and Gen-4 video generation models right from your conversational workspace. Produce stunning, realistic, or highly stylized video clips simply by typing out your vision or providing a reference image.

### What you can do

- **Text-to-Video Generation** — Write detailed prompts to synthesize entirely new, imaginative scenes using `gen3_turbo`, `gen4_turbo`, or the standard `text_to_video` tooling.
- **Image-to-Video Animation** — Bring still images to life using `image_to_video` or precisely guide the motion of a starting image with a textual director prompt using `image_text_to_video`.
- **Advanced Interpolation** — Seamlessly blend two distinct keyframe images into one smooth transitional motion clip (`interpolate`).
- **Complete Task Management** — Maintain full control over costly generation pipelines. Easily check job status or output URLs (`get_task`, `list_tasks`), cancel ongoing renders to save credits (`cancel_task`), and audit your organization's billing usage (`get_organization`).

### How it works

1. Successfully enable the Runway ML integration within this application hub.
2. Sign into your Runway Developer Portal and access the API Keys section.
3. Once you generate a new, secure token, paste it securely into the connection configuration below.
4. Chat with your AI: "Generate a 10 second cinematic video of a futuristic cyberpunk city using Gen-3 Turbo."

### Who is this for?

- **Creative Directors & Media Teams** — Develop storyboards, conceptualize scenes, or rapidly prototype full commercial grade sequences inside simple textual conversations.
- **Social Content Creators** — Generate eye-catching B-roll quickly using high-grade diffusion models exactly tailored directly from prompt instructions.


## Available Tools (10)
- **get_task**: Look for SUCCEEDED status and output URL.

Retrieves the status and output of a generation task
- **image_text_to_video**: Generates video from both an image and a text prompt
- **image_to_video**: Specify source image URL, model, and duration.

Animates a still image into a video
- **interpolate**: Creates smooth motion between two keyframe images
- **list_tasks**: Lists recent generation tasks
- **text_to_video**: Specify prompt, model, and duration (5 or 10). Returns a task ID.

Generates a video from a text prompt
- **cancel_task**: This action is irreversible.

Cancels a running generation task
- **gen3_turbo**: Quick 5-second video generation using Gen-3 Alpha Turbo
- **gen4_turbo**: High-quality video generation using Gen-4 Turbo
- **get_organization**: Retrieves Runway ML organization and credit details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runway ML** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 5 second cinematic video showing a sunset over an alien planet using Runway Gen-3 Turbo."

**🤖 AI Agent:**
> Your Runway generation task was successfully submitted to the Gen-3 Turbo model. The task ID is rw_task_1234. You can ask me to poll this task in a moment to review the final video output.

---

**👤 You:**
> "Take this reference image URL and animate it with Gen-3 Turbo to make the camera slowly pan backwards."

**🤖 AI Agent:**
> Image to video request initiated using the `image_text_to_video` tool. Your task is now processing and I got the ID 'rw_task_9876'. The animation will be ready shortly.

---

**👤 You:**
> "List all my ongoing tasks on Runway to see if the video has finished rendering."

**🤖 AI Agent:**
> I've scanned your recent 10 tasks. I see that task 'rw_task_1234' just SUCCEEDED! Here is the MP4 link to your generated video.


## ❓ FAQ

**Q: How can I preview the output without fully committing my prompt?**
Video generation actions using the Runway engines are directly invoked through asynchronous background tasks. Instead of an exact real-time preview, you can start small 5-second generations or iterate closely on your prompt texts until they produce the final aesthetic you want.

**Q: Does this integration process video rendering in real-time?**
No. Video rendering is asynchronous. When you submit a prompt or an image, the AI will dispatch a background task to Runway's servers and receive a 'task_id'. You will need to ask the AI to verify the status of this task later, usually after a few minutes, to fetch the final video URL.

**Q: Can I use Gen-4 models for free?**
No. Runway requires credits for all generations, and Gen-4 Turbo consumes significantly more credits than earlier models or standard actions. You must maintain sufficient active credits or a paid subscription on your Runway account for the AI to successfully execute the rendering jobs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-ml](https://vinkius.com/mcp/runway-ml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runway ML** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runway-ml` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runway ML** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runway-ml": {
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
