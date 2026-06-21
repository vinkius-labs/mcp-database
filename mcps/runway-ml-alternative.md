# Runway ML MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-ml-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/runway-ml-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/runway-ml-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Automate AI video generation via Runway ML — create, monitor, and manage Gen-3 Alpha and Gen-2 tasks directly from any AI agent.

## Description
Connect your **Runway ML** account to any AI agent to automate high-end video generation workflows through natural conversation.

### What you can do

- **Advanced Generation** — Trigger Gen-3 Alpha Turbo or Gen-2 models using text prompts or image-to-video inputs
- **Precise Control** — Configure duration (5s or 10s), aspect ratios, seeds, and watermarking for professional results
- **Real-time Monitoring** — Query specific task statuses and retrieve output URLs as soon as the AI finishes processing
- **Asset Management** — List your entire generation history and delete or cancel tasks to keep your workspace organized

### How it works

1. Subscribe to this server
2. Enter your Runway API Key
3. Start generating cinematic videos from Claude, Cursor, or any MCP-compatible client

No more manual checking of generation progress bars. Your AI agent acts as a creative director, handling the technical API calls while you focus on the vision.

### Who is this for?

- **Creative Directors** — quickly iterate on visual concepts and storyboards without leaving the chat interface
- **Content Creators** — automate the production of video assets by describing scenes in natural language
- **Developers** — integrate professional video generation capabilities directly into your coding workflow or internal tools


## Available Tools
- **create_task**: Create a new Runway generation task
- **delete_task**: Delete a Runway task
- **get_task**: Retrieve a Runway task
- **list_tasks**: List Runway tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runway ML** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Gen-3 Alpha Turbo video of a rainy cyberpunk street, 10 seconds long, 1280:768 ratio."

**🤖 AI Agent:**
> I've initiated the generation task. Your Task ID is '7a8b9c-d1e2-f3g4'. I'll monitor the status for you.

---

**👤 You:**
> "Check the progress of my Runway task with ID '7a8b9c-d1e2-f3g4'."

**🤖 AI Agent:**
> The task is currently 'SUCCEEDED'. You can view your video here: [Output URL].

---

**👤 You:**
> "List all my recent video generation tasks."

**🤖 AI Agent:**
> I've retrieved your task list. You have 5 recent tasks, including 'Cyberpunk Street' (Succeeded) and 'Mountain Sunset' (Succeeded).


## Installation & Usage

To install and use the **Runway ML** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-ml-alternative](https://vinkius.com/mcp/runway-ml-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
