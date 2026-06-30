# Runway ML MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-ml-alternative)
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


## Available Tools (4)
- **delete_task**: Delete a Runway task
- **get_task**: Retrieve a Runway task
- **create_task**: Create a new Runway generation task
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


## ❓ FAQ

**Q: How do I start a new video generation with a specific prompt?**
Use the `create_task` tool. You can specify the model (like `gen3a_turbo`), the `promptText`, and even optional parameters like `duration` (5 or 10 seconds) or `ratio`.

**Q: How can I check if my video is ready to download?**
Use the `get_task` tool with your unique task ID. It will return the current status and the output URL once the generation is complete.

**Q: Is it possible to remove a task from my history or stop a running one?**
Yes, the `delete_task` tool allows you to cancel an active generation or remove the record of a completed task from your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-ml-alternative](https://vinkius.com/mcp/runway-ml-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `runway-ml-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runway ML** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runway-ml-alternative": {
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
