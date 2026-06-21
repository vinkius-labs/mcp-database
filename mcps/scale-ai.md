# Scale AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scale-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Automate high-quality data labeling and RLHF workflows via Scale AI — create projects, manage batches, and submit annotation tasks directly from your AI agent.

## Description
Connect your **Scale AI** account to any AI agent to orchestrate large-scale data labeling and fine-tuning pipelines through natural conversation.

### What you can do

- **Project Management** — Create and configure projects for specific labeling types like image annotation or semantic segmentation.
- **Batch Operations** — Organize high-volume work into batches and finalize them to trigger the labeling process.
- **Multi-Modal Tasks** — Submit tasks for Image Annotation, Semantic Segmentation, and Video Playback directly via API.
- **Task Lifecycle** — Retrieve detailed status of individual tasks or cancel pending ones to manage your budget and throughput.
- **Parameter Tuning** — Update project-level instructions and parameters dynamically to refine labeling quality.

### How it works

1. Subscribe to this server
2. Enter your Scale AI Live API Key
3. Start managing your data pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — automate the submission of edge cases for labeling directly from training scripts or analysis notebooks.
- **Data Operations Managers** — monitor batch progress and update labeling instructions without leaving the chat interface.
- **AI Researchers** — quickly spin up RLHF or annotation projects to validate new model datasets.


## Available Tools
- **cancel_task**: Optionally clears the unique_id to reuse it.

Cancel a pending task
- **create_batch**: Create a new batch
- **create_image_annotation_task**: Create an Image Annotation task
- **create_named_entity_recognition_task**: Create a Named Entity Recognition task
- **create_project**: Create a new Scale project
- **create_segment_annotation_task**: Create a Semantic Segmentation task
- **create_text_collection_task**: Create a Text Collection task
- **create_video_playback_annotation_task**: Create a Video Annotation task
- **finalize_batch**: Finalize a batch
- **get_task**: Retrieve a specific task
- **update_project_params**: Update project parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scale AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new image annotation project called 'Lidar-Obstacles' for imageannotation."

**🤖 AI Agent:**
> I've created the project 'Lidar-Obstacles'. You can now start creating batches or submitting tasks to this project.

---

**👤 You:**
> "Submit an image annotation task to project 'Lidar-Obstacles' with the image URL 'https://example.com/car.jpg'."

**🤖 AI Agent:**
> Task created successfully. The Task ID is 'task_abc123'. You can track its progress using the get_task tool.

---

**👤 You:**
> "Finalize the batch named 'sprint-01-batch'."

**🤖 AI Agent:**
> Batch 'sprint-01-batch' has been finalized. Scale will now begin processing the tasks within this batch.


## ❓ FAQ

**Q: How do I start a high-volume labeling job using batches?**
First, use `create_batch` to initialize a group for your project. After submitting your tasks to this batch, call `finalize_batch` to signal Scale to begin the labeling process.

**Q: Can I check the status of a specific annotation task?**
Yes, use the `get_task` tool with the specific Task ID. It will return the full metadata, current status, and any available results for that unit of work.

**Q: What should I do if I submitted a task by mistake?**
You can use the `cancel_task` tool with the Task ID. If you need to reuse the unique identifier, you can also set the `clear_unique_id` parameter to true.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scale-ai](https://vinkius.com/mcp/scale-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scale AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `scale-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scale AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scale-ai": {
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
