# Zenodo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenodo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zenodo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zenodo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage scientific research and datasets on Zenodo—create depositions, upload files, and search records directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenodo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for public Zenodo records related to 'machine learning in healthcare'."

**🤖 AI Agent:**
> I've found several records. The most relevant include 'Dataset for ML in Clinical Diagnosis' (ID: 789012) and 'Survey of Healthcare AI' (ID: 345678). Would you like more details on any of these?

---

**👤 You:**
> "Create a new Zenodo deposition for a dataset titled 'Global Temperature Trends 2023'."

**🤖 AI Agent:**
> I've created a new unpublished deposition for you. The Deposition ID is 1234567. You can now start adding creators or uploading files to this draft.

---

**👤 You:**
> "List all files currently attached to my deposition with ID 987654."

**🤖 AI Agent:**
> Checking deposition 987654... I found 3 files: 'raw_data.csv', 'analysis_script.py', and 'metadata.json'. Would you like to update any of these or add more?


## Installation & Usage

To install and use the **Zenodo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenodo](https://vinkius.com/mcp/zenodo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
