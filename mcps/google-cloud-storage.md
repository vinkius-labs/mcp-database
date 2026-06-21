# Google Cloud Storage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-storage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your GCS buckets and objects — list files, upload data, and audit permissions via AI.

## Description
Connect your **Google Cloud Storage** project to your AI agent and streamline your cloud data management. Use natural language to browse buckets, inspect file metadata, manage object lifecycles, and audit security permissions across your global storage infrastructure.

### What you can do

- **Bucket Exploration** — List all buckets in your project and retrieve detailed metadata including location and storage class
- **Object Management** — Browse files within buckets using prefixes (folders), view sizes, and delete or copy objects effortlessly
- **Data Operations** — Upload text-based content directly or initiate object copies between buckets via simple commands
- **Security Auditing** — Check Access Control Lists (ACLs) and IAM policies for both buckets and individual objects to ensure compliance
- **Project Insights** — Retrieve service account details and manage HMAC keys for legacy or cross-cloud integrations

### How it works

1. Subscribe to this server
2. Enter your Google Cloud Project ID and OAuth credentials
3. Complete the secure Google Cloud authorization flow
4. Start managing your cloud storage from Claude, Cursor, or any MCP-compatible client

No more manual navigation through the GCP Console for routine file checks. Your AI agent acts as your cloud storage administrator, handling the JSON API for you.

### Who is this for?

- **Cloud Engineers** — quickly check if a specific build artifact or log file exists in a bucket without opening the console
- **Data Scientists** — browse datasets and verify file sizes or modification dates via natural language
- **Security Teams** — audit bucket permissions and public access settings instantly through conversational queries


## Available Tools
- **copy_object**: Copy an object within or between buckets
- **delete_object**: Remove an object from a bucket
- **get_bucket_iam**: Get IAM policy for a bucket
- **get_bucket_metadata**: Get metadata for a specific bucket
- **get_object_metadata**: Get metadata for a specific object (file)
- **get_project_service_account**: Check the storage service account for the project
- **list_bucket_acl**: Check bucket permissions
- **list_buckets**: List all buckets in the project
- **list_hmac_keys**: List HMAC keys for a service account
- **list_object_acl**: Check permissions for a specific object
- **list_objects**: List objects within a bucket
- **upload_object**: Upload a new file to a bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Storage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all buckets in my Google Cloud project."

**🤖 AI Agent:**
> Retrieving buckets... You have 4 buckets: 1. 'prod-assets-9302', 2. 'staging-logs-backup', 3. 'user-uploads-data', 4. 'temp-exports'. Would you like the metadata for the 'prod-assets' bucket?

---

**👤 You:**
> "Find all files in bucket 'prod-assets' that start with 'images/2024/'."

**🤖 AI Agent:**
> Browsing objects... I found 15 objects with that prefix. Notable files include 'logo-v1.png', 'hero-background.jpg', and 'icon-set.svg'. Would you like to see the metadata for 'logo-v1.png'?

---

**👤 You:**
> "Check who has access to the 'user-uploads-data' bucket."

**🤖 AI Agent:**
> Auditing bucket ACL... The 'user-uploads-data' bucket is restricted to internal service accounts and specific team members (admins). Public access ('allUsers') is currently NOT granted. Would you like the full IAM policy details?


## ❓ FAQ

**Q: Can I upload large files directly through this server?**
The `upload_object` tool is designed for small to medium text-based content. For very large binary files or production datasets, it is recommended to use the gsutil CLI or the Google Cloud Console to ensure optimal transfer speeds and integrity.

**Q: How do I check if a bucket is publicly accessible?**
You can use the `list_bucket_acl` or `get_bucket_iam` tools. The AI agent will retrieve the permissions and can identify if roles like 'allUsers' or 'allAuthenticatedUsers' have been granted access.

**Q: Can I move files between different buckets?**
Yes! Use the `copy_object` tool to copy an object from a source bucket to a destination bucket. To 'move' it, you would typically copy the object first and then use `delete_object` on the source.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-storage](https://vinkius.com/mcp/google-cloud-storage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Cloud Storage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-cloud-storage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Cloud Storage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-cloud-storage": {
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
