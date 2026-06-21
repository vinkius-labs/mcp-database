# Uploadcare MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uploadcare)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uploadcare-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uploadcare-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your entire media infrastructure — upload, retrieve, organize, and delete files securely via Uploadcare directly from your AI agent.

## Description
Connect your **Uploadcare** account to any AI agent to fully manage your file handling and CDN media infrastructure via natural conversation.

### What you can do

- **File Management** — List uploaded assets, retrieve specific file technical metadata (like dimensions and CDN URLs), and manage permanent storage states.
- **Bulk Operations** — Efficiently batch store or batch delete multiple temporary or permanent files in a single operation.
- **File Transport** — Copy existing files manually to local or remote storage targets, directly through your AI agent.
- **Groups & Collections** — List immutable file collections (groups) and inspect which individual files are contained within them.
- **Project Analytics** — Retrieve your Uploadcare project-level metadata, checking your current account storage and bandwidth consumption in real time.

### How it works

1. Subscribe to this server
2. Enter your Uploadcare Public and Secret Keys
3. Start managing your media infrastructure from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes the control center for your media distribution platform.

### Who is this for?

- **Software Engineers** — debug upload issues, quickly retrieve CDN URLs, and inspect file technical metadata without opening the dashboard.
- **Content Managers** — clean up unused assets, organize file groups, and permanently delete massive batches of files using just natural language.
- **DevOps Teams** — monitor project storage limits, bandwidth usage, and automate the copying of files to external S3 buckets.
- **Product Teams** — audit recent user uploads and ensure temporary unneeded files aren't taking up storage quotas.


## Available Tools
- **batch_delete_files**: This action is irreversible.

Permanently removes multiple files in a single operation
- **batch_store_files**: Marks multiple temporary files as permanently stored
- **copy_file**: g. S3).

Copies an existing file to local or remote storage
- **delete_file**: This action is irreversible.

Permanently removes a file and its variants from Uploadcare
- **get_file_details**: Retrieves technical metadata for a specific Uploadcare file
- **get_group_details**: Retrieves information about a specific file group
- **get_project_info**: Retrieves project-level metadata and usage statistics
- **list_files**: Supports pagination via limit.

Lists files stored in your Uploadcare project
- **list_file_groups**: Lists immutable file collections (groups) in the project
- **store_file**: Marks a temporary file as permanently stored


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uploadcare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current project storage and bandwidth usage?"

**🤖 AI Agent:**
> Based on your project info, you currently have 15.2 GB stored across 45,120 active files. Your bandwidth for this billing period is at 230 GB. This places you at 85% of your current plan limits. Would you like me to inspect and list the largest files so we can batch delete some test data?

---

**👤 You:**
> "Can you check the dimensions and CDN URL for file UUID `9cd83...`?"

**🤖 AI Agent:**
> I checked the asset. It's a `hero-banner.jpg` (mime_type: image/jpeg) weighing 2.4MB. It is currently marked as permanently stored. Its dimensions are 3840x2160 pixels. The raw public CDN access url is `https://ucarecdn.com/9cd83.../`. Let me know if you want me to copy this to an S3 bucket.

---

**👤 You:**
> "Batch delete these 4 outdated temporary images: `e33b...`, `f55a...`, `8c11...`, `ab99...`."

**🤖 AI Agent:**
> I've successfully executed the `batch_delete_files` command. All 4 assets (`e33b...`, `f55a...`, `8c11...`, `ab99...`) and their related CDN variants have been irrevocably deleted from your Uploadcare project. Your storage limits have been safely reduced.


## Installation & Usage

To install and use the **Uploadcare** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uploadcare](https://vinkius.com/mcp/uploadcare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
