# Zenodo MCP Server

Manage scientific research and datasets on Zenodo—create depositions, upload files, and search records directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zenodo)

## Overview
**Category:** knowledge-management
**Tools Count:** 14

## Description
Connect your **Zenodo** account to any AI agent to streamline your scientific research workflows and data management through natural conversation.

### What you can do

- **Deposition Management** — Create new unpublished depositions, update metadata, and manage your research drafts directly from the AI.
- **Record Discovery** — Search and list public records across the entire Zenodo database to find relevant research, software, or datasets.
- **File Inspection** — List all files attached to specific depositions to understand the contents of a research package.
- **Metadata Control** — Precisely update titles, creators, descriptions, licenses, and access rights for your unpublished work.
- **Version Tracking** — Retrieve specific deposition details using unique IDs to monitor the status of your submissions.

### How it works

1. Subscribe to this server
2. Enter your Zenodo Personal Access Token
3. Start managing your research data from Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex forms to update a dataset description or find a specific research record. Your AI acts as a dedicated research assistant.

### Who is this for?

- **Researchers & Academics** — quickly draft depositions and manage metadata for publications without leaving your writing environment.
- **Data Scientists** — automate the listing and retrieval of datasets for analysis directly from your code editor.
- **Open Science Advocates** — easily search and discover public research artifacts to foster collaboration and transparency.


## Available Tools
- **create_deposition**: You can optionally provide metadata.

Create a new Zenodo deposition
- **delete_deposition_file**: Delete a file from a Zenodo deposition
- **delete_deposition**: Note: Only unpublished depositions can be deleted.

Delete an unpublished Zenodo deposition
- **discard_deposition**: Discard edits on a Zenodo deposition
- **edit_deposition**: Edit a published Zenodo deposition
- **get_deposition**: Retrieve a Zenodo deposition by ID
- **get_record**: Retrieve a published Zenodo record by ID
- **list_deposition_files**: List files in a Zenodo deposition
- **list_depositions**: List Zenodo depositions
- **list_records**: Search published Zenodo records
- **new_version_deposition**: Create a new version of a Zenodo deposition
- **publish_deposition**: WARNING: Once published, a deposition cannot be deleted.

Publish a Zenodo deposition
- **update_deposition**: Update a Zenodo deposition
- **upload_deposition_file**: Upload a text file to a Zenodo deposition


## Installation & Usage

To install and use the **Zenodo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenodo](https://vinkius.com/mcp/zenodo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
