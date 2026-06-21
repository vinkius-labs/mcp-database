# Aliyun OSS / 阿里云对象存储 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aliyun-oss)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aliyun-oss-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aliyun-oss-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading object storage service — manage files, buckets, and metadata via AI.

## Description
Empower your AI agent to orchestrate your cloud storage and asset management with **Aliyun OSS** (对象存储), the dominant object storage provider in China. By connecting Aliyun OSS to your agent, you transform complex file operations, bucket auditing, and metadata management into a natural conversation. Your agent can instantly upload text assets, retrieve detailed object metadata, list bucket contents with prefix filtering, and monitor storage status without you ever needing to navigate the comprehensive Aliyun Console. Whether you are conducting a digital asset audit or coordinating a content refresh, your agent acts as a real-time cloud storage assistant, providing accurate and fast results from a single, authorized source.

### What you can do

- **Asset Orchestration** — Upload, delete, and manage text-based objects across your Aliyun OSS buckets.
- **Metadata Auditing** — Retrieve detailed HTTP headers and custom metadata for any stored object.
- **Bucket Management** — List objects with advanced filtering (prefix, marker) and verify bucket locations.
- **Public URL Generation** — Automatically generate public endpoints for your shared assets.
- **System Monitoring** — Monitor bucket configuration and API connectivity to ensure operational health.

### How it works

1. Subscribe to this server
2. Enter your Aliyun AccessKey ID, AccessKey Secret, Endpoint, and Bucket Name
3. Start managing your cloud assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate asset deployments and monitor storage configurations through natural language queries.
- **Content Operations** — manage media metadata and coordinate asset refreshes directly from your AI-powered workspace.
- **Developers** — integrate professional cloud storage APIs into your AI-driven daily routines.
- **Aliyun Power Users** — integrate your existing OSS workflows into your AI-driven daily routines.


## Available Tools
- **copy_object**: Uses x-oss-copy-source header.

Copy an object within the bucket
- **delete_object**: Delete an object from OSS
- **download_object_text**: Best for text/JSON files.

Download an object as text
- **get_bucket_acl**: Get bucket access control list
- **get_bucket_info**: Get bucket configuration
- **get_bucket_location**: g., oss-cn-hangzhou) where your bucket is located.

Get bucket region
- **get_bucket_statistics**: Get bucket storage statistics
- **get_object_metadata**: Get object metadata (HEAD)
- **list_objects**: Use prefix to filter by path, marker for pagination.

List objects in the bucket
- **upload_object**: Max 5GB per request.

Upload text content to OSS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aliyun OSS / 阿里云对象存储** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all objects in my Aliyun OSS bucket with prefix 'images/'."

**🤖 AI Agent:**
> I've retrieved the object list for your bucket. I found 15 items under the 'images/' prefix, including 'banner.jpg' and 'logo.png'. Would you like me to get the detailed metadata for any of these files?

---

**👤 You:**
> "Upload this text to 'config/settings.json': '{"theme": "dark"}'."

**🤖 AI Agent:**
> I've successfully uploaded the JSON content to your OSS bucket at the key `config/settings.json`. The object is now stored securely. Would you like me to verify the upload by retrieving its metadata?

---

**👤 You:**
> "What is the public URL for 'docs/manual.pdf'?"

**🤖 AI Agent:**
> The public URL for your object is: `https://[bucket].[endpoint].aliyuncs.com/docs/manual.pdf`. Note that this URL will only work if the object has been granted 'public-read' permissions in your bucket settings.


## Installation & Usage

To install and use the **Aliyun OSS / 阿里云对象存储** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aliyun-oss](https://vinkius.com/mcp/aliyun-oss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
