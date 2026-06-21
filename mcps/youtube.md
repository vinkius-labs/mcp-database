# YouTube MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/youtube)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search for videos, retrieve detailed statistics, and audit channel performance on YouTube — the world's leading video sharing platform.

## Description
Connect your **YouTube Data API** account to any AI agent and harness the power of global video intelligence through natural conversation.

### What you can do

- **Universal Search** — Find relevant video content by keyword or exact phrase, retrieving a list of metadata including titles and descriptions
- **Deep Video Insights** — Retrieve full technical metadata for specific videos, including view counts, like counts, and engagement statistics
- **Channel Performance** — Monitor any YouTube channel's branding and statistics, including total subscriber counts and video volume
- **Sentiment Analysis** — Fetch the most relevant comments from any video to analyze user feedback and community engagement
- **Content Discovery** — Quickly find unique video and channel IDs required for automated media monitoring workflows
- **Trend Auditing** — Browse and analyze video descriptions and statistics to identify content patterns and audience interests
- **Metadata Retrieval** — Get high-resolution thumbnails and precise upload timestamps for any piece of video content

### How it works

1. Subscribe to this server
2. Enter your YouTube API Key (from Google Cloud Console)
3. Start querying video data through Claude, Cursor, or any MCP-compatible client

No more manual searching through the YouTube interface to find an engagement metric. Your AI agent becomes your video data analyst.

### Who is this for?

- **Marketing Managers** — monitor channel growth and audit video engagement metrics through simple chat commands
- **Content Creators** — analyze competitor performance and retrieve relevant user comments for sentiment feedback
- **Data Scientists** — collect video metadata and statistics for trend analysis without building custom scrapers
- **Research Teams** — quickly surface relevant video content and verify channel branding through conversation


## Available Tools (4)
- **get_video**: Retrieves full metadata, description, and statistics for a specific YouTube video
- **search_videos**: Returns a list of video metadata including titles and descriptions.

Search for YouTube videos by keyword or exact phrase
- **get_channel**: Retrieves complete statistics and branding information for a YouTube channel
- **list_comments**: Returns the most recent/relevant comment threads.

Fetches the top most relevant comments from a specific YouTube video


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YouTube** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search YouTube for 'generative AI tutorials' and show me the top 5 results."

**🤖 AI Agent:**
> I found the top 5 videos for 'generative AI tutorials'. Highlights include: 1. 'GenAI for Beginners' (ID: abc-123), 2. 'Advanced LLM Prompting' (ID: def-456), and 3. 'Building with Stable Diffusion' (ID: ghi-789). Which one would you like the full details for?

---

**👤 You:**
> "What are the statistics for video ID 'dQw4w9WgXcQ'?"

**🤖 AI Agent:**
> Video 'Never Gonna Give You Up' (ID: dQw4w9WgXcQ) has 1.5 billion views, 17 million likes, and approximately 2.1 million comments. It was uploaded on Oct 25, 2009. Would you like me to list the latest comments?

---

**👤 You:**
> "Check the subscriber count for channel ID 'UC_x5XG1OV2P6uYZ5M1D2ogw'."

**🤖 AI Agent:**
> The channel 'Google for Developers' (ID: UC_...) currently has 2.45 million subscribers and a total of 1,250 videos. The total view count across all videos is approximately 450 million.


## ❓ FAQ

**Q: Can I see how many likes and views a video has through the agent?**
Yes. The `get_video_details` tool allows your AI agent to retrieve full real-time statistics for any YouTube video ID, including view counts, like counts, and the total number of comments.

**Q: How do I find out the subscriber count for a specific channel?**
You can use the `get_channel_details` tool. Provide the unique channel ID, and your agent will return the channel's performance statistics, including subscriber counts, total views, and video counts.

**Q: Is it possible to read the comments on a video via chat?**
Absolutely. Use the `list_video_comments` tool to retrieve the top most relevant or recent comment threads from any video ID, helping you perform rapid sentiment analysis through conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/youtube](https://vinkius.com/mcp/youtube)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **YouTube** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `youtube` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **YouTube** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "youtube": {
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
