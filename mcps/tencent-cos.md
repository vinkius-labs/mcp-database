# Tencent COS / 腾讯云对象存储 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-cos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tencent-cos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tencent-cos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's dominant cloud storage platform — manage files, metadata, and CDN endpoints via AI.

## Description
Empower your AI agent to orchestrate your cloud storage infrastructure and asset management with **Tencent COS** (对象存储), the premier storage service in China. By connecting Tencent COS to your agent, you transform complex file operations, metadata auditing, and storage lifecycle management into a natural conversation. Your agent can instantly upload text assets, retrieve detailed object headers, list directory contents with delimiter support, and monitor storage status without you ever needing to navigate the comprehensive Tencent Cloud Console. Whether you are conducting a digital asset audit or coordinating a content update, your agent acts as a real-time cloud storage coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Asset Orchestration** — Upload, delete, and manage text-based objects across your Tencent COS buckets.
- **Metadata Auditing** — Retrieve detailed HTTP headers and verify object existence through secure metadata queries.
- **Inventory Control** — List objects with advanced filtering (prefix, delimiter) to organize your storage structure.
- **Public URL Generation** — Automatically generate public endpoints for your shared cloud assets.
- **System Monitoring** — Verify bucket configuration and API connectivity to ensure operational continuity.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId, SecretKey, Region, and Bucket Name
3. Start managing your cloud assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate asset deployments and monitor storage health through natural language queries.
- **Operations Managers** — manage media metadata and coordinate content refreshes directly from your AI-powered workspace.
- **Developers** — integrate professional cloud storage APIs into your AI-driven daily routines.
- **Tencent Cloud Power Users** — integrate your existing COS workflows into your AI-driven daily routines.


## Available Tools
- **check_object_exists**: Check if an object exists
- **copy_object**: Copy an object within the bucket
- **delete_object**: Delete an object from COS
- **download_object_text**: Download an object as text
- **get_bucket_acl**: Get bucket access permissions
- **get_object_metadata**: Get object metadata (HEAD)
- **head_bucket**: Check if the bucket exists and is accessible
- **list_objects**: Use prefix to filter by path.

List objects in the COS bucket
- **list_root_objects**: List top-level objects and folders
- **upload_object**: Max 5GB per request.

Upload text content to COS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent COS / 腾讯云对象存储** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in the root of my Tencent COS bucket."

**🤖 AI Agent:**
> I've retrieved the root object list. I found 10 items, including 'index.html' and 'uploads/'. Would you like to see the contents of a specific folder or get metadata for a file?

---

**👤 You:**
> "Check if the file 'backups/db_init.sql' exists in COS."

**🤖 AI Agent:**
> I've performed a metadata check for that key. The file `backups/db_init.sql` exists in your bucket. It was created on Oct 27, 2023 and has a size of 1.2 MB. Should I generate a public URL for it?

---

**👤 You:**
> "Get the metadata for 'static/css/main.css'."

**🤖 AI Agent:**
> I've retrieved the metadata for that object. The Content-Type is 'text/css' and it has an ETag of '88210934...'. The storage class is Standard. Would you like me to download the text content for you to audit?


## Installation & Usage

To install and use the **Tencent COS / 腾讯云对象存储** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-cos](https://vinkius.com/mcp/tencent-cos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
