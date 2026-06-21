# Amazon S3 Bucket MCP Server

Single-bucket object storage for AI agents — scoped access to one S3 bucket for secure, focused data operations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-s3-bucket)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Grant your AI agent **precise, scoped access** to a single Amazon S3 bucket — no more, no less. Unlike full S3 access, this integration enforces the principle of least privilege: your agent can read, write, and manage objects exclusively within one pre-configured bucket.

### What you can do

- **Browse Objects** — List and navigate files within the bucket using prefix and delimiter filters
- **Read Data** — Retrieve object contents or inspect metadata (headers, content type, size) without downloading
- **Write Data** — Upload string or JSON content as objects directly into the bucket
- **Clean Up** — Delete specific objects to maintain storage hygiene
- **Audit Security** — Inspect the bucket's access policy and ACL to ensure compliance

### How it works

1. Subscribe to this server
2. Enter your AWS Access Key, Secret Key, Region, and the **target Bucket Name**
3. Your agent operates exclusively within that bucket — no access to other buckets or account-level operations

### Why single-bucket?

AI agents should follow the **principle of least privilege**. Granting full S3 access to an autonomous agent creates unnecessary blast radius. This server confines the agent to a single bucket, which means:
- No accidental bucket creation or deletion
- No cross-bucket data exposure
- Clearer audit trail for compliance
- Safer agent-to-agent delegation

### Who is this for?

- **AI Engineers** — give each agent a dedicated data workspace without exposing your entire cloud storage
- **Data Teams** — let agents process, query, and write results to a specific data lake partition
- **Platform Engineers** — enforce tenant isolation by assigning one bucket per agent or workflow
- **Security-Conscious Teams** — minimize attack surface by scoping storage access to exactly what's needed


## Available Tools
- **delete_object**: Delete an object
- **get_bucket_acl**: Get bucket ACL
- **get_bucket_policy**: Get bucket policy
- **get_object_data**: Get object content
- **get_object_metadata**: Get object metadata
- **list_objects**: Can be filtered by prefix and delimiter.

List objects in the bucket
- **put_object**: Upload an object


## Installation & Usage

To install and use the **Amazon S3 Bucket** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-s3-bucket](https://vinkius.com/mcp/amazon-s3-bucket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
