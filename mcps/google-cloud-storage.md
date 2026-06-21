# Google Cloud Storage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-storage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-cloud-storage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-cloud-storage-mcp)
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


## Installation & Usage

To install and use the **Google Cloud Storage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-storage](https://vinkius.com/mcp/google-cloud-storage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
