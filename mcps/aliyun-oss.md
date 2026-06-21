# Aliyun OSS / 阿里云对象存储 MCP Server

China's leading object storage service — manage files, buckets, and metadata via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aliyun-oss)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Aliyun OSS / 阿里云对象存储** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aliyun-oss](https://vinkius.com/mcp/aliyun-oss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
