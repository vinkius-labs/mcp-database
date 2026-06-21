# Roboflow MCP Server

Manage computer vision workflows — upload images, train models, and manage datasets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/roboflow)

## Overview
**Category:** developer-tools
**Tools Count:** 29

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


## Available Tools
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


## Installation & Usage

To install and use the **Roboflow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roboflow](https://vinkius.com/mcp/roboflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
