# Scale AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scale-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scale-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scale-ai-mcp)
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


## Installation & Usage

To install and use the **Scale AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scale-ai](https://vinkius.com/mcp/scale-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
