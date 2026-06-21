# Qiniu Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qiniu-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qiniu-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qiniu-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Qiniu Cloud storage — manage buckets, handle file uploads, and monitor CDN performance directly from any AI agent.

## Description
Connect your AI agents to **Qiniu Cloud** (七牛云), the leading enterprise cloud storage and content delivery network in China. This MCP provides 10 tools to manage the full lifecycle of your cloud assets, from bucket orchestration and file manipulation to CDN cache refreshment and global traffic monitoring.

### What you can do

- **Storage Orchestration** — List buckets and manage file lifecycles, including deletions and bulk operations
- **File Management** — Retrieve granular metadata for stored assets and generate download URLs programmatically
- **CDN Optimization** — Refresh cache and prefetch content to ensure high-performance delivery across the network
- **Usage Analytics** — Monitor bandwidth consumption and storage quotas directly through natural conversation

### How it works

1. Subscribe to this server
2. Log in to the [**Qiniu Cloud Console**](https://portal.qiniu.com/)
3. Navigate to **Access Key** settings in your profile
4. Copy your **AccessKey** and **SecretKey**
5. Insert your credentials into the fields below to start managing your Qiniu cloud infrastructure.

### Who is this for?

- **Infrastructure Engineers** — automate the management of large-scale cloud storage buckets
- **Media Developers** — monitor asset delivery and trigger CDN refreshes programmatically
- **DevOps Teams** — track cloud consumption and manage storage quotas efficiently


## Available Tools
- **delete_file**: Delete a file from a bucket
- **get_account_info**: Retrieve Qiniu account profile
- **get_bucket_domains**: Get domains associated with a specific bucket
- **get_cdn_bandwidth**: Get CDN bandwidth statistics
- **get_file_stat**: Get metadata for a specific file
- **get_pfop_status**: Check the status of a persistent processing task
- **get_sms_stats**: Get SMS sending statistics
- **list_buckets**: List all storage buckets in your Qiniu account
- **list_files**: List files within a bucket
- **persistent_file_op**: Trigger persistent file processing (transcoding, etc.)
- **refresh_cdn_urls**: Refresh CDN cache for specific URLs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qiniu Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all storage buckets in my Qiniu account."

**🤖 AI Agent:**
> Retrieving your Qiniu buckets... I found 3 active buckets: 1. media-assets, 2. static-web, 3. user-backups. Which one would you like to inspect?

---

**👤 You:**
> "Get the file status for 'logo.png' in bucket 'media-assets'."

**🤖 AI Agent:**
> Querying file metadata... 'logo.png' (ID: abc123hash) has a size of 45KB and is set to type 'image/png'. It was last modified on 2024-04-10.

---

**👤 You:**
> "Refresh the CDN cache for 'https://cdn.example.com/styles.css'."

**🤖 AI Agent:**
> Connecting to Qiniu Fusion CDN... Refresh request submitted successfully! The cache for your CSS file is being purged across all global nodes.


## Installation & Usage

To install and use the **Qiniu Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qiniu-cloud](https://vinkius.com/mcp/qiniu-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
