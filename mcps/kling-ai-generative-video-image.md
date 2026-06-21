# Kling AI (Generative Video & Image) MCP Server

Generate cinematic videos and images via Kling AI — use text-to-video, image-to-video, and AI virtual try-on.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kling-ai-generative-video-image)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Kling AI (Generative Video & Image)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kling-ai-generative-video-image](https://vinkius.com/mcp/kling-ai-generative-video-image)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
