# Google Cloud Storage Bucket MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-storage-bucket)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-cloud-storage-bucket-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-cloud-storage-bucket-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages files in a single Google Cloud Storage Bucket. That's its only function, and nothing else. Incredible for giving your AI secure file storage.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to read, write, and list files inside one specific GCS Bucket.**

By strictly scoping access, your AI can safely persist data, analyze documents, and manage its own workload without ever touching your critical cloud infrastructure.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single bucket. It cannot list other buckets or delete your company's production backups.
- **Native GCP Integration:** Direct, high-performance interactions with Google Cloud using Service Account credentials.
- **Plug & Play File System:** Instantly gives your agent a massive cloud hard drive to store its memories, generated assets, and processed reports.


## Available Tools
- **delete_object**: Delete an object from the Google Cloud Storage bucket
- **get_object**: Read the content of an object in the Google Cloud Storage bucket
- **list_objects**: List objects in the configured Google Cloud Storage bucket
- **put_object**: If the object already exists, it is overwritten.

Upload or overwrite an object in the Google Cloud Storage bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Storage Bucket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files inside the 'data/exports/' folder."

**🤖 AI Agent:**
> I found 3 files with the prefix 'data/exports/': export-1.csv, export-2.csv, and summary.json.

---

**👤 You:**
> "Upload this JSON configuration to 'configs/agent-settings.json'."

**🤖 AI Agent:**
> I've successfully uploaded the JSON data to 'configs/agent-settings.json' with `content-type: application/json`.

---

**👤 You:**
> "Delete the temporary 'processing/job-123.tmp' file."

**🤖 AI Agent:**
> The file 'processing/job-123.tmp' was successfully deleted from the Google Cloud Storage bucket.


## Installation & Usage

To install and use the **Google Cloud Storage Bucket** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-storage-bucket](https://vinkius.com/mcp/google-cloud-storage-bucket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
