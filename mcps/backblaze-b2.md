# Backblaze B2 MCP Server

Manage Backblaze B2 Cloud Storage via AI — control buckets, file versions, objects, and access rules autonomously.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/backblaze-b2)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Connect your **Backblaze B2** account to any AI agent and manage your cloud storage architecture directly through natural conversation.

### O que você pode fazer

- **Buckets** — Create, delete, update privacy (allPrivate/allPublic), and list globally mapped storage buckets
- **File Management** — Hide files (soft delete), remove explicit file versions (hard delete), and list surface names
- **Health Validation** — List unfinished large file chunks to find failed multipart uploads
- **File Intelligence** — Retrieve granular file details, sizes, hashes (SHA1), and content types natively

### Como funciona

1. Subscribe to this server
2. Enter your Backblaze B2 Application Key ID and Key
3. Start architecting storage and debugging files from Claude, Cursor, or any MCP-compatible client

Your AI agent now has the power to orchestrate secure and cost-effective object storage without leaving your editor.

### Para quem é?

- **DevOps Engineers** — rapidly verify bucket states, clean up abandoned file versions, and debug failed multipart streams
- **Backend Developers** — create public and private storage domains directly from development spaces
- **System Administrators** — audit object footprint securely and perform granular file integrity checks


## Available Tools
- **authorize_account**: Uncovers the dynamically assigned apiUrl (e.g. api003.backblazeb2.com) natively orchestrating regional data ingress specifically assigned to your billing account.

Verify and extract Backblaze global session routing endpoints
- **create_bucket**: Bootstraps essential structures before assigning automated backup syncs overriding file lock retention bounds.

Provision a fresh logical Storage Bucket partition
- **delete_bucket**: Fails intentionally via 400 Bad Request if standard files or hidden object versions persist nested inside. Ensure all lifecycle rules completed purging prior to command.

Irreversibly delete an entirely empty Backblaze Storage Bucket
- **delete_file_version**: Instantly removes the storage footprint avoiding long-term retention hoarding.

Irreversibly vaporize specific absolute chunk data from disk arrays
- **get_file_info**: Obtain granular checksum and headers associated with one precise B2 File
- **hide_file**: Does not actually delete binary payload, merely injects a null-marker shadowing the actual file ensuring b2_list_file_names ignores it, enforcing safe soft deletion logic.

Mark an active B2 file as hidden leaving data for lifecycle sweep
- **list_buckets**: Crucial to resolve immutable String Bucket IDs prerequisite to executing downstream CRUD operations strictly inside native borders.

Retrieve the exact Storage Buckets existing globally on the B2 Account
- **list_file_names**: Examines precise .pdf, .mp4 file locations avoiding hidden shadowed states produced by lifecycle overwrite semantics.

Paginate primary surface-level object metadata from a specific Bucket
- **list_unfinished_large_files**: Crucial for verifying broken API pipelines originating from external S3 clients failing CompleteMultipartUpload.

Scan B2 nodes for stalled Multipart Upload chunk aggregates
- **update_bucket**: Use only for static asset endpoints.

Mutate global ACL privacy settings for a bounded Bucket


## Installation & Usage

To install and use the **Backblaze B2** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/backblaze-b2](https://vinkius.com/mcp/backblaze-b2)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
