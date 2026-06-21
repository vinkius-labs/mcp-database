# UPYUN Developer Platform MCP Server

Bring UPYUN's Massive CDN and Image Processing APIs to your AI. Interact with buckets and deploy files to the cloud.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/upyun-developer-platform)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 5

## Description
Integrate your AI with **UPYUN** (又拍云), one of the most prominent Cloud and CDN providers in the world. This MCP gives your agent direct file management access to your cloud buckets.

### What you can do

- **Cloud Storage Management** — Automatically create, view, list, and delete files inside your UPYUN buckets without downloading their manual command line clients
- **CDN Artifact Uploads** — Enable the LLM to directly write code logic or textual artifacts and deploy them live to your CDN domains instantly
- **Capacity Auditing** — Fetch storage usage to monitor consumption on your buckets dynamically

### How it works

1. Subscribe to this server
2. Obtain an Operator Name and Password inside your bucket's API access page
3. Plug the credentials into your agent and you are fully connected. The MCP abstracts away the legacy HMAC-SHA1 Authorization header generation securely.

### Who is this for?

- **DevOps Agents** — Automate static site generation and deployments directly pushing file changes to UPYUN instances
- **Frontend Engineers** — Skip writing complex Python deploy scripts when prototyping web applications
- **Content Administrators** — Check what is currently inside specific UPYUN directories via natural language


## Available Tools
- **create_text_file**: Create and upload a text file directly to UPYUN
- **delete_file**: Delete a file from UPYUN
- **get_file_info**: Get metadata about an UPYUN file
- **get_service_usage**: Get UPYUN bucket service usage
- **list_directory**: g., "/" or "/images/") to list its contents.

List files and folders in an UPYUN directory


## Installation & Usage

To install and use the **UPYUN Developer Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upyun-developer-platform](https://vinkius.com/mcp/upyun-developer-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
