# Tavus Video Replicas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tavus-video-replicas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate personalized AI videos via Tavus — manage replicas, create videos from scripts, and track generation status.

## Description
Connect your AI agent to **Tavus**, the leading platform for automated personalized video generation. This integration allows you to leverage AI replicas to create high-quality, talking-head videos for sales, marketing, and customer success directly from your conversation.

### What you can do

- **Replica Management** — List and inspect your trained AI video replicas
- **Video Generation** — Create new videos by providing a script and selecting a replica
- **Status Tracking** — Monitor the progress of video generation tasks in real-time
- **Content Library** — Access a list of all your generated videos and their download links
- **Resource Cleanup** — Permanently delete replicas or videos no longer needed

### How it works

1. Subscribe to this server
2. Enter your **Tavus API Key** (v2)
3. Start generating personalized video content through natural language

### Who is this for?

- **Marketing Teams** — automate the creation of personalized video campaigns at scale
- **Sales Professionals** — generate custom outreach videos for prospects using AI clones
- **Customer Success** — create personalized onboarding and support videos for clients


## Available Tools
- **delete_replica**: Permanently delete a specific replica
- **delete_video**: Permanently delete a specific generated video
- **generate_replica_video**: Generate a new AI video using a specific replica
- **get_replica_details**: Get comprehensive details for a specific replica
- **get_video_details**: Get detailed information for a specific generated video
- **list_replicas**: Retrieve a list of all your AI video replicas
- **list_generated_videos**: Retrieve a list of all generated videos


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tavus Video Replicas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Tavus replicas."

**🤖 AI Agent:**
> Fetching replicas... I found 2 replicas: 'Sales Persona' (ID: rep_123) and 'Founder Clone' (ID: rep_456). Both are ready for use.

---

**👤 You:**
> "Generate a video with replica 'rep_123' saying 'Hello, welcome to our platform!'."

**🤖 AI Agent:**
> Generation task started! Video ID is 'vid_789'. You can check the status in a few minutes to get the download link.


## ❓ FAQ

**Q: How do I create a replica?**
Replicas currently must be initiated via the Tavus Dashboard or their specific training endpoints which require a source video. This agent allows you to manage and use existing replicas.

**Q: How long does video generation take?**
Personalized video generation typically takes a few minutes depending on the length of the script. You can use the `get_video_details` tool to check if the status is 'completed'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tavus-video-replicas](https://vinkius.com/mcp/tavus-video-replicas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tavus Video Replicas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tavus-video-replicas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tavus Video Replicas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tavus-video-replicas": {
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
