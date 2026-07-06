# Spiritme MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spiritme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Create AI-generated videos with digital human presenters that deliver personalized messages in multiple languages naturally.

## Description
Connect your **Spiritme** account to any AI agent and take full control of your automated video avatar generation and high-fidelity personalized media workflows through natural conversation.

### What you can do

- **Avatar Portfolio Orchestration** — List and manage your entire high-fidelity portfolio of digital avatars programmatically, retrieving detailed technical metadata and SKU IDs
- **Video Generation Intelligence** — Programmatically trigger and monitor high-fidelity video generation jobs using custom scripts and voice selections
- **Asset & Media Architecture** — Access your complete directory of high-fidelity hosted video assets to oversee your organizational resource allocation in real-time
- **Engagement Monitoring** — Access real-time status updates for video processing and track generation results directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor video orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Spiritme dashboard (Settings > API)
3. Start orchestrating your video growth from Claude, Cursor, or any MCP client

No more manual recording of video updates or missing critical avatar generation status. Your AI acts as your dedicated media coordinator and video architect.

### Who is this for?

- **Content Marketers** — instantly trigger personalized video messages and monitor job status using natural language commands
- **Training Teams** — verify individual avatar metadata and track training video generation without leaving your creative workspace
- **Developers** — integrate high-speed Spiritme avatar data into custom automated video pipelines through simple AI queries


## Available Tools (12)
- **get_avatar**: Get avatar details
- **get_job_status**: Get video job status
- **get_template**: Get template details
- **get_voice**: Get voice details
- **list_avatars**: List avatars
- **list_templates**: List templates
- **list_videos**: List videos
- **list_voices**: List voices
- **check_spiritme_status**: Verify connectivity
- **delete_video**: Delete a video
- **generate_audio**: Generate audio
- **generate_video**: Generate a video


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spiritme** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a video with avatar 'av_123' and script: 'Hello, welcome to our team!'."

**🤖 AI Agent:**
> Video orchestrated! I've successfully submitted the generation request for avatar av_123. The job ID is job_xyz789. The high-fidelity video will be ready shortly. Shall I notify you once the status is 'Completed'?

---

**👤 You:**
> "Check the status of video job 'job_xyz789'."

**🤖 AI Agent:**
> Job intelligence orchestrated! For job_xyz789, the current high-fidelity status is 'DONE'. The video was generated successfully at 2:00 PM today. Need help retrieving the final hosted URL?

---

**👤 You:**
> "List all active videos in my Spiritme library."

**🤖 AI Agent:**
> Asset directory orchestrated! I've retrieved your high-fidelity video portfolio. You currently have 10 active assets, including 'Intro 2024' and 'Product Update'. Would you like the detailed technical metadata for any of them?


## ❓ FAQ

**Q: How do I find my Spiritme API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I check the status of a video job via AI?**
Yes! The `get_spiritme_job_status` tool allows your agent to poll the high-fidelity real-time status of any generation request.

**Q: How do I list my available avatars?**
Use the `list_spiritme_avatars` tool to retrieve your complete high-fidelity directory along with the unique identifiers for all managed digital actors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spiritme](https://vinkius.com/mcp/spiritme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spiritme** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spiritme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spiritme** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spiritme": {
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
