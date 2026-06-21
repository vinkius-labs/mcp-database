# Qiniu Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qiniu-cloud)
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


## ❓ FAQ

**Q: Can I automatically list all buckets in my Qiniu account?**
Yes! Use the `list_buckets` tool. Your agent will retrieve a complete list of all Kodo storage buckets currently configured in your account.

**Q: How do I refresh the CDN cache for a specific URL?**
Use the `refresh_cdn` tool with a list of target URLs. This will trigger the Qiniu Fusion CDN to purge the old cached versions and fetch the latest assets.

**Q: Can I retrieve metadata for a specific file?**
Yes! Use the `get_file_stat` tool with the bucket name and file key. Your agent will return the file size, hash, and MIME type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qiniu-cloud](https://vinkius.com/mcp/qiniu-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qiniu Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qiniu-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qiniu Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qiniu-cloud": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
