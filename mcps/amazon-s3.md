# Amazon S3 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-s3)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-s3-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-s3-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Cloud object storage orchestration — manage buckets, objects, and metadata via AI.

## Description
Connect your **Amazon S3** environment to your AI agent to unlock professional cloud storage orchestration. From creating and auditing buckets to managing individual objects and their metadata, your agent handles your AWS data storage through natural conversation.

### What you can do

- **Bucket Orchestration** — List your S3 buckets, create new ones, and retrieve their location or policy configurations
- **Object Management** — List objects within a specific bucket, including their size and last modified timestamps
- **Data Ingestion** — Upload objects directly to S3 or delete unwanted files to maintain your storage hygiene
- **Metadata Auditing** — Retrieve technical metadata (headers, content type, size) for specific objects without downloading them
- **Security Oversight** — Audit bucket ACLs and policies to ensure your cloud storage meets compliance requirements

### How it works

1. Subscribe to this server
2. Enter your AWS Access Key, Secret Key, and Region
3. Start managing your cloud storage and monitoring your data assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Cloud Engineers** — automate bucket audits and verify object configurations effortlessly
- **Data Scientists** — quickly find specific datasets or list objects in your data lake directly from chat
- **DevOps Specialists** — monitor S3 policies and manage file cleanups using simple commands
- **Security Analysts** — audit bucket access controls and identify exposed data via API queries


## Available Tools
- **list_buckets**: List S3 buckets
- **create_bucket**: Create an S3 bucket
- **delete_bucket**: Delete an S3 bucket
- **list_objects**: Can be filtered by prefix.

List objects in bucket
- **get_object_metadata**: Get object metadata
- **get_object_data**: Get object content
- **put_object**: Upload an object
- **delete_object**: Delete an object
- **get_bucket_policy**: Get bucket policy
- **get_bucket_acl**: Get bucket ACL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon S3** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all S3 buckets in my account."

**🤖 AI Agent:**
> I've retrieved your S3 buckets. You currently have 4 buckets: 'production-assets', 'backup-logs-2026', 'website-images-eu', and 'data-lake-raw'. Would you like me to list the contents of the 'production-assets' bucket?

---

**👤 You:**
> "Show the top 10 objects in bucket 'data-lake-raw' starting with prefix '2026/03/'."

**🤖 AI Agent:**
> I've listed the objects matching that prefix. I found 10 files, mostly CSV and JSON logs. The largest file is '2026/03/15/transactions.csv' at 25MB. Would you like to see the metadata for that specific file?

---

**👤 You:**
> "Get the bucket policy for 'website-images-eu'."

**🤖 AI Agent:**
> I've retrieved the policy for 'website-images-eu'. The bucket currently has a public read policy attached (`s3:GetObject` allowed for `*`). Are you sure this bucket should be publicly accessible?


## Installation & Usage

To install and use the **Amazon S3** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-s3](https://vinkius.com/mcp/amazon-s3)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
