# Google Cloud Storage MCP Server

Manage your GCS buckets and objects — list files, upload data, and audit permissions via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-storage)

## Overview
**Category:** industry-titans
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Google Cloud Storage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-storage](https://vinkius.com/mcp/google-cloud-storage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
