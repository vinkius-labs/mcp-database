# Runway ML MCP Server

Empower your AI with Runway ML's advanced video generation capabilities to seamlessly create, animate, and interpolate high-quality clips using Gen-3 and Gen-4 Turbo models directly from chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-ml)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

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


## Available Tools
- **cancel_task**: This action is irreversible.

Cancels a running generation task
- **gen3_turbo**: Quick 5-second video generation using Gen-3 Alpha Turbo
- **gen4_turbo**: High-quality video generation using Gen-4 Turbo
- **get_organization**: Retrieves Runway ML organization and credit details
- **get_task**: Look for SUCCEEDED status and output URL.

Retrieves the status and output of a generation task
- **image_text_to_video**: Generates video from both an image and a text prompt
- **image_to_video**: Specify source image URL, model, and duration.

Animates a still image into a video
- **interpolate**: Creates smooth motion between two keyframe images
- **list_tasks**: Lists recent generation tasks
- **text_to_video**: Specify prompt, model, and duration (5 or 10). Returns a task ID.

Generates a video from a text prompt


## Installation & Usage

To install and use the **Runway ML** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-ml](https://vinkius.com/mcp/runway-ml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
