# Wasabi MCP Server

Manage buckets, objects, and versioning on Wasabi — the hot cloud storage for high-performance data residency.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wasabi)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Wasabi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wasabi](https://vinkius.com/mcp/wasabi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
