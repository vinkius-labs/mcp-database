# Wasabi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wasabi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage buckets, objects, and versioning on Wasabi — the hot cloud storage for high-performance data residency.

## Description
Connect your **Wasabi Hot Cloud Storage** account to any AI agent and take full control of your cloud assets through natural conversation.

### What you can do

- **Bucket Management** — List all storage buckets, create new ones, or delete obsolete containers in your account
- **Object Discovery** — Browse and list files (objects) stored within specific buckets, including sizes and last modified dates
- **Data Integrity** — Enable and check bucket versioning to protect against accidental file overwrites or deletions
- **Access Control** — Audit permissions and retrieve Access Control Lists (ACL) for specific files to ensure security
- **Data Residency** — Verify the physical geographic region where your data is hosted for compliance needs
- **Cleanup Tasks** — Identify fractured file uploads that consume storage and permanently delete obsolete assets

### How it works

1. Subscribe to this server
2. Enter your Wasabi Access Key, Secret Key, and Region
3. Start managing your cloud storage through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex storage consoles to check your files. Your AI agent becomes your cloud storage administrator.

### Who is this for?

- **Cloud Architects** — verify data residency compliance and manage storage buckets across different regions
- **Data Engineers** — browse datasets, manage object versions, and cleanup incomplete multipart uploads
- **DevOps Professionals** — automate bucket provisioning and audit file access permissions through chat
- **IT Administrators** — monitor storage containers and manage data lifecycle policies with simple commands


## Available Tools (10)
- **create_storage_bucket**: Provide a globally unique lower-kebab-case name.

Creates a new high-availability storage bucket in the configured Wasabi region
- **delete_storage_bucket**: Note: The bucket must be completely empty first. This action is irreversible.

Permanently removes an empty storage bucket
- **delete_bucket_object**: This action is irreversible.

Permanently deletes a specific file from a bucket
- **enable_bucket_versioning**: Activates object versioning for a bucket
- **get_bucket_datacenter_location**: Retrieves the physical geographic region where a bucket is hosted
- **get_object_access_control**: Retrieves the access control list (ACL) for a specific file
- **get_bucket_versioning_status**: Checks if object versioning is enabled for a bucket
- **list_storage_buckets**: Lists all Wasabi storage buckets visible to the authenticated IAM user
- **list_bucket_objects**: Returns file keys, sizes, and last modified dates.

Lists the files (objects) stored within a specific bucket
- **list_pending_multipart_uploads**: Lists incomplete multipart uploads in a bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wasabi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my storage buckets in Wasabi."

**🤖 AI Agent:**
> I found 3 buckets in your account: 'backups-2026' (Created: 2026-01-15), 'user-data-prod' (Created: 2025-11-20), and 'media-assets-global' (Created: 2026-02-10). Would you like to see the contents of any of these?

---

**👤 You:**
> "What files are inside the 'backups-2026' bucket?"

**🤖 AI Agent:**
> Searching 'backups-2026'… I found 5 objects: 'db-dump-jan.sql' (4.2 GB), 'logs-archive.zip' (850 MB), 'config-backup.json' (12 KB), and 2 others. I can pull the ACL or delete any of these for you.

---

**👤 You:**
> "Is versioning enabled for my 'user-data-prod' bucket?"

**🤖 AI Agent:**
> Checking status… No, object versioning is currently suspended for 'user-data-prod'. Would you like me to enable it now to protect your files from accidental overwrites?


## ❓ FAQ

**Q: Can I check if a file is publicly accessible through the agent?**
Yes. The `get_object_access_control` tool allows your AI agent to retrieve the Access Control List (ACL) for any specific file, helping you audit permissions and identify public objects.

**Q: How do I protect my files from accidental deletion in a bucket?**
You can use the `enable_bucket_versioning` tool to activate versioning on your bucket. This ensures that historical copies of your files are preserved, allowing you to recover from accidental overwrites or deletions.

**Q: Can I see where my data is physically stored?**
Absolutely. Use the `get_bucket_datacenter_location` tool to retrieve the specific geographic region where a bucket is hosted, ensuring you meet data residency requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wasabi](https://vinkius.com/mcp/wasabi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wasabi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wasabi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wasabi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wasabi": {
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
