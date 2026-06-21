# Twelve Labs (Video Understanding) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twelve-labs-video-understanding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Search, analyze, and extract semantic insights from video content using Twelve Labs' powerful multimodal AI models.

## Description
Connect **Twelve Labs** to your AI agent to unlock the full potential of video understanding. This server allows your agent to index video files, perform complex semantic searches, and generate deep analytical insights from visual and audio data.

### What you can do

- **Video Indexing** — Create and manage indexes to organize your video library for rapid retrieval and analysis.
- **Semantic Search** — Query your video content using natural language to find specific moments, objects, or actions without manual tagging.
- **Asset Management** — Upload videos via URLs or multipart sessions and monitor their indexing status in real-time.
- **Deep Analysis** — Run synchronous or asynchronous analysis tasks to extract structured data from your video assets.
- **Embeddings & Entities** — Generate multimodal embeddings and manage entity collections for advanced machine learning workflows.

### How it works

1. Subscribe to this server
2. Enter your Twelve Labs API Key
3. Start querying your video data from Claude, Cursor, or any MCP-compatible client

Transform your video archives into searchable, actionable data. Your AI can now 'watch' and understand hours of footage in seconds.

### Who is this for?

- **Content Creators & Media Teams** — quickly find b-roll or specific scenes across massive video libraries.
- **Security & Operations** — search through hours of footage for specific events or objects using natural language.
- **Developers** — integrate state-of-the-art video understanding into your AI workflows without building complex pipelines.


## Available Tools
- **analyze_async**: Analyze and segment videos asynchronously
- **analyze_sync**: Analyze and segment videos synchronously
- **confirm_multipart_upload**: Confirm a multipart upload
- **create_asset**: Upload content to create an asset
- **create_entity_collection**: Create an entity collection
- **create_entity**: g., a person) within a collection.

Create an entity
- **create_index**: Create a new index
- **create_multipart_upload**: Create a multipart upload session
- **delete_index**: Delete an index
- **embed_async**: Create embeddings asynchronously
- **embed_sync**: Create embeddings synchronously
- **get_index**: Retrieve an index by ID
- **get_indexed_asset**: Retrieve an indexed asset
- **index_asset**: Index an uploaded asset
- **list_indexes**: List all indexes
- **report_multipart_progress**: Report progress for a multipart upload
- **search**: Search for moments in videos
- **update_index**: Update an index name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twelve Labs (Video Understanding)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Twelve Labs video indexes."

**🤖 AI Agent:**
> I've retrieved your indexes. You have 3 active indexes: 'Marketing-2024' (ID: idx_abc123), 'Product-Demos' (ID: idx_def456), and 'Security-Feed' (ID: idx_ghi789).

---

**👤 You:**
> "Create a new index named 'Webinar-Archive' using the Marengo 3.0 model with visual and audio options."

**🤖 AI Agent:**
> Index 'Webinar-Archive' has been created successfully with ID: idx_web987. It is configured with the Marengo 3.0 model for both visual and audio analysis.

---

**👤 You:**
> "Search for 'a person presenting a slideshow' in index idx_abc123."

**🤖 AI Agent:**
> Searching... I found 2 relevant matches in index idx_abc123. The first is at 02:15 in 'Q3-Review.mp4' and the second is at 10:45 in 'Strategy-Session.mp4'.


## ❓ FAQ

**Q: How do I list all my existing video indexes?**
You can use the `list_indexes` tool. It will return a list of all indexes available in your Twelve Labs account, including their IDs and configuration.

**Q: Can I search for a specific moment inside my videos using text?**
Yes! Use the `search` tool by providing an `index_id` and a search query. The AI will find the most relevant timestamps and video segments based on your description.

**Q: How do I add a new video to an index for analysis?**
First, use `create_asset` with a public URL to upload the video. Then, use the `index_asset` tool with the resulting `asset_id` and your target `index_id` to start the processing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twelve-labs-video-understanding](https://vinkius.com/mcp/twelve-labs-video-understanding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twelve Labs (Video Understanding)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `twelve-labs-video-understanding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twelve Labs (Video Understanding)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twelve-labs-video-understanding": {
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
