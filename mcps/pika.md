# Pika MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pika)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pika-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pika-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Equip your AI agent with Pika Labs native video generation. Create text-to-video, animate images, generate sound effects, and lip-sync programmatically.

## Description
Connect your **Pika 2.2** fal.ai endpoint to your AI agent and construct a massive programmatic video production studio relying solely on natural language commands.

### What you can do

- **Video Generation** — Turn raw language concepts perfectly into high-fidelity video scenes applying `generate_video_from_text`, or use `generate_video_with_duration` to specify specific clip timing.
- **Image Animation** — Revitalize stagnant 2D images by using `animate_image` and `interpolate_keyframes` to build professional fluid motion sequences.
- **Post-Production Effects** — Morph characters dynamically using `apply_visual_effects` to add squish, melt, and deflation rendering directly via chat.
- **Audio Capabilities** — Instruct your AI to compose targeted soundscapes using `generate_sound_effects`, or perfectly align vocal dubs to characters utilizing `lip_sync_video`.
- **Job Control** — Queue heavy programmatic generations, and poll their render completion employing `get_job_status` and `get_job_result` directly from the terminal.

### How it works

1. Subscribe to this server
2. Enter your Fal.ai Authentication Token (which securely routes to the Pika Labs backend)
3. Prompt your favorite AI (Claude, Cursor) to act as a movie director and start producing HD mp4 sequences

### Who is this for?

- **Content Creators & Agencies** — write a script conceptually, have the AI outline scenes, and immediately trigger the Pika generation endpoints sequentially.
- **Game Developers** — easily animate static asset drops (textures and splashes) and compose synthetic sound effects on the fly via command interactions.
- **Film Tinkerers** — orchestrate fully automated movie storyboards rendering exact camera pans and lip-sync dubs completely inside your IDE workflow.


## Available Tools
- **generate_video_from_text**: 2 foundation node.

Generate a video from a text prompt using Pika Labs 2.2 via fal.ai. Pika creates cinematic AI videos with smooth motion. Returns request_id for async polling. Instructions: Pass prompt. Poll get_job_status for completion
- **animate_image**: Animate a still image into a video using Pika Labs 2.2. Brings photos to life with AI-generated motion. Instructions: Pass image URL and prompt for motion direction
- **generate_multi_image_scene**: Create multi-reference video scenes using Pika Scenes. Combines multiple images into a coherent video. Instructions: Pass comma-separated image URLs and prompt
- **interpolate_keyframes**: Create smooth interpolation between keyframe images using Pika Frames. Generates transitional video between 2+ keyframes. Instructions: Pass comma-separated image URLs and prompt
- **apply_visual_effects**: Apply visual effects to an image using Pika Effects. Transforms images with cinematic effects. Instructions: Pass image URL and effect type
- **get_job_status**: ai ledgers confirm render bounds.

Get the status of a Pika generation request. Returns status (IN_QUEUE/IN_PROGRESS/COMPLETED). Instructions: Poll until COMPLETED
- **get_job_result**: Get the final result of a completed Pika generation. Returns video URL and metadata. Instructions: Call after status is COMPLETED
- **generate_video_with_duration**: Generate video with duration control using Pika 2.2. Specify exact duration in seconds. Instructions: Pass prompt and duration
- **lip_sync_video**: Lip-sync a video to audio using Pika Labs. Matches mouth movements to speech. Instructions: Pass video URL and audio URL
- **generate_sound_effects**: Generate AI sound effects for a video using Pika Labs. Auto-detects scene and adds appropriate SFX. Instructions: Pass video URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pika** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 5-second video of a cyberpunk city floating in neon clouds."

**🤖 AI Agent:**
> The video generation has been queued internally (ID: pk-1029). I'll check its status over the next couple of minutes and alert you when the asset is completely processed.

---

**👤 You:**
> "Apply the 'melt' visual effect to the job ID pk-1029."

**🤖 AI Agent:**
> I've invoked the `apply_visual_effects` tool with the 'melt' parameter on source asset pk-1029. A new task has spawned to calculate this destruction scene.

---

**👤 You:**
> "Check the status of task pk-1029 and fetch the video link if it's done."

**🤖 AI Agent:**
> I pinged `get_job_status` and it returned 'COMPLETED'. Using `get_job_result`, here is the final MP4 hyperlink: [https://fal.media/cloud/...]


## Installation & Usage

To install and use the **Pika** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pika](https://vinkius.com/mcp/pika)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
