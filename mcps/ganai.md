# GAN.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ganai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate personalized videos at scale, track generation status, and oversee campaigns via AI agents with GAN.ai.

## Description
Connect your **GAN.ai** account to any AI agent to automate your personalized video marketing and sales outreach through the Model Context Protocol (MCP). GAN.ai is a leading generative AI platform that enables brands to create thousands of unique videos with custom names, locations, and details. This MCP server enables you to trigger video generation, monitor real-time processing status, and retrieve landing page links directly through natural conversation.

### Key Features

- **Personalized Video Generation** — Trigger bulk video generation based on project templates and dynamic tags (e.g., first name, company).
- **Real-time Status Monitoring** — Track the asynchronous processing of your video requests and retrieve final MP4 and landing page URLs.
- **Project Oversight** — List all video templates/projects and fetch detailed variable definitions for personalization.
- **Campaign Discovery** — Access your history of generated videos and monitor their status (pending, processing, completed).
- **Landing Page Integration** — Retrieve branded landing page permalinks for each generated video to fuel your outreach sequences.
- **Engagement Analytics** — Fetch view counts and engagement metrics for specific videos to measure campaign success.
- **Webhook Visibility** — List configured webhooks to ensure your systems are receiving real-time generation notifications.
- **Real-time Synchronization** — Keep your generative video strategy accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GAN Workspace ID and API Token (found in your Settings)
3. Start managing your personalized video generation from Claude, Cursor, or any MCP client

### Who is this for?

- **Growth Marketers** — quickly trigger personalized video campaigns for new leads without manual dashboard uploads.
- **Sales Development Reps (SDRs)** — get a real-time status of custom videos for prospects via simple AI commands.
- **Content Operations** — automate the retrieval of video metadata and analytics for reporting.


## Available Tools
- **verify_api_connection**: ai API connectivity.

Verify API access
- **generate_personalized_videos**: Generate videos in bulk
- **generate_single_video**: Generate one video
- **get_workspace_info**: ai workspace.

Get workspace details
- **get_project_metadata**: Get template schema
- **get_video_stats**: Get engagement stats
- **get_video_metadata**: Get video details
- **get_generation_status**: Check video status
- **list_landing_templates**: List landing pages
- **list_video_projects**: List video templates
- **list_generated_videos**: List video history
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GAN.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available video projects in GAN.ai."

**🤖 AI Agent:**
> Retrieving projects... I found 3 active projects: 'Welcome Message v2', 'Product Demo', and 'Follow-up Campaign'. Which template should we use?

---

**👤 You:**
> "Generate a personalized video for 'John Doe' (johndoe@email.com) using project 'proj_123'."

**🤖 AI Agent:**
> Generation triggered! I've successfully sent the request for John Doe. The Inference ID is 'inf_abc789'. I'll monitor its status for you.

---

**👤 You:**
> "Check the status of video generation 'inf_abc789'."

**🤖 AI Agent:**
> Checking status... The video for John Doe is 'Completed'! You can access the personalized landing page here: [Permalink].


## ❓ FAQ

**Q: How do I find my Workspace ID and API Token?**
Log in to GAN.ai, go to Settings, and navigate to the API section to find your Workspace ID and generate a Bearer Token.

**Q: What is an 'Inference ID'?**
An Inference ID is a unique tracking number returned when you trigger a video generation. You use it with the 'get_generation_status' tool to check if the video is ready.

**Q: Are personalized landing pages included in the API response?**
Yes! Once a video is completed, the agent retrieves the 'permalink', which is a non-expiring link to the personalized landing page hosting the video.

**Q: Can I monitor video view analytics via the agent?**
Yes, the 'get_video_stats' tool allows you to retrieve real-time engagement data, such as view counts and playback metrics, for any generated video.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ganai](https://vinkius.com/mcp/ganai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GAN.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ganai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GAN.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ganai": {
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
