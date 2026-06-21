# Roboflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roboflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage computer vision workflows — upload images, train models, and manage datasets directly from your AI agent.

## Description
Connect **Roboflow** to your AI agent to streamline your computer vision pipeline. From dataset management to model training and inference, handle your entire CV lifecycle through natural language.

### What you can do

- **Workspace & Project Management** — List projects, create new ones, or fork from Roboflow Universe to jumpstart your development.
- **Dataset Operations** — Upload images (via URL or Base64), manage versions, and download datasets in various formats like COCO or YOLO.
- **Model Training** — Start training runs, monitor results, and retrieve precise performance metrics (mAP, precision, recall) for any version.
- **Image Search** — Search and filter images within your workspace to audit your data and improve model accuracy.
- **Inference & Results** — Run inference on images and retrieve results to verify model behavior in real-time.

### How it works

1. Subscribe to this server
2. Enter your Roboflow Private API Key
3. Start building and managing vision models from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **ML Engineers** — monitor training progress and dataset health without leaving the terminal or IDE.
- **Data Scientists** — quickly query dataset versions and export data for custom training scripts.
- **Product Teams** — audit model performance and visualize inference results through simple conversation.


## Available Tools (29)
- **add_projects_to_folder**: Add projects to a folder (Enterprise)
- **auto_label**: Start an auto-labeling job using foundation models
- **cancel_training**: Cancel an active training job
- **create_annotation_job**: Assign a batch of images to a labeler and reviewer
- **create_folder**: Create a project folder (Enterprise)
- **create_project**: Create a new project in a workspace
- **delete_images**: Delete multiple images from a project
- **delete_project**: Delete a project or version (moves to Trash)
- **download_dataset**: Retrieve a download link for a zipped dataset in a specific format
- **fork_universe_project**: Fork a public project from Roboflow Universe
- **get_async_task**: Track long-running operations like forking or large exports
- **get_dataset_health**: Check dataset health (class distribution, missing annotations, etc)
- **get_image**: Get details for a specific image
- **get_project**: Get project details, metadata, and versions
- **get_root**: Verify authentication and retrieve default workspace
- **get_training_results**: Retrieve metrics and status for a version training run
- **get_version**: Retrieve metadata for a specific dataset version
- **list_folders**: List project folders in a workspace (Enterprise)
- **list_trash**: List items in the workspace trash
- **list_workspace_projects**: List information about a workspace and its projects
- **manage_image_tags**: Add, remove, or set tags on an image
- **restore_trash**: Restore an item from the trash
- **run_inference**: Run inference on an image using hosted models
- **search_project_images**: Search and filter images within a specific project
- **search_workspace_images**: Search and filter images within a workspace
- **start_training**: Start training a model on a dataset version
- **stop_training**: Early stop an active training job
- **upload_annotation**: Attach an annotation file to an existing image
- **upload_image**: Upload an image to a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roboflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Roboflow workspace 'industrial-safety'."

**🤖 AI Agent:**
> I've retrieved the projects for 'industrial-safety'. You have 3 active projects: 'Hard Hat Detection' (object-detection), 'Glove Compliance' (classification), and 'Forklift Tracking'. Which one would you like to inspect?

---

**👤 You:**
> "Upload this image URL to the 'Hard Hat Detection' project in workspace 'industrial-safety'."

**🤖 AI Agent:**
> Uploading image... Success! The image has been added to the 'Hard Hat Detection' project. It is currently in the unassigned batch. Would you like to assign it to a specific split?

---

**👤 You:**
> "Show me the training metrics for version 5 of the 'Forklift Tracking' project."

**🤖 AI Agent:**
> Fetching results for version 5... The model achieved a mAP of 88.5%, with a precision of 91.2% and recall of 84.7%. The training run is completed. Would you like to see the full metrics breakdown?


## ❓ FAQ

**Q: How can I verify if my Roboflow API key is correctly configured?**
You can use the `get_root` tool. It will attempt to authenticate with your key and return the default workspace details if successful.

**Q: Can I get the training performance metrics for a specific model version?**
Yes! Use the `get_training_results` tool by providing the workspace, project, and version ID. It returns mAP, precision, recall, and other training metrics.

**Q: Is it possible to export my dataset to a specific format like YOLOv5?**
Absolutely. Use the `download_dataset` tool and specify the `format` parameter (e.g., 'yolov5pytorch') to receive a download link for your zipped dataset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roboflow](https://vinkius.com/mcp/roboflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roboflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roboflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roboflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roboflow": {
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
