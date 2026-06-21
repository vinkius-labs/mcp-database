# Luma AI (Generative Video & Creative) MCP Server

Generate cinematic AI videos and images via Luma — use Dream Machine for text-to-video, image-to-video, and professional camera control.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/luma-ai-generative-video-creative)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Luma AI (Generative Video & Creative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/luma-ai-generative-video-creative](https://vinkius.com/mcp/luma-ai-generative-video-creative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
