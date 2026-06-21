# Amazon S3 Bucket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-s3-bucket)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Single-bucket object storage for AI agents — scoped access to one S3 bucket for secure, focused data operations.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon S3 Bucket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in this bucket."

**🤖 AI Agent:**
> I've listed the contents of your bucket. You have 12 objects, including 3 CSV files in the 'reports/' prefix and 5 JSON logs under 'events/2026/'. The largest file is 'reports/annual-summary.csv' at 18 MB. Would you like me to retrieve the content of a specific file?

---

**👤 You:**
> "Upload this JSON config to 'settings/app-config.json'."

**🤖 AI Agent:**
> Done! I've uploaded the JSON configuration to 'settings/app-config.json' in your bucket. The object is now available at that key. Would you like me to verify the upload by retrieving the metadata?

---

**👤 You:**
> "Check the access policy on this bucket."

**🤖 AI Agent:**
> I've retrieved the bucket policy. The current configuration allows read access from a specific IAM role and denies all public access. The bucket also has server-side encryption (AES-256) enforced on all PUT operations. Your setup looks secure. Would you like me to also check the ACL?


## ❓ FAQ

**Q: How is this different from the full Amazon S3 server?**
The full Amazon S3 server gives the agent access to all buckets in your AWS account — it can list, create, and delete buckets. This server scopes the agent to a single, pre-configured bucket. The agent can only read, write, and manage objects within that bucket. This follows the principle of least privilege, which is critical for secure agent deployments.

**Q: How do I get my AWS Access Key and Secret Key?**
Log in to the AWS Management Console, navigate to IAM (Identity and Access Management), and create a user with programmatic access. For this integration, we recommend a policy scoped to a single bucket (e.g., `s3:GetObject`, `s3:PutObject`, `s3:DeleteObject`, `s3:ListBucket` limited to your target bucket ARN).

**Q: Can I upload large files using this integration?**
The `put_object` tool handles standard REST uploads and is best suited for small to medium-sized files or JSON data. For very large files, standard AWS tools utilizing Multipart Uploads are recommended.

**Q: Can my agent access multiple buckets?**
Each instance of this server is scoped to exactly one bucket. If your agent needs access to multiple buckets, you can subscribe to this server multiple times — each with a different bucket configuration. This maintains strict isolation between data boundaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-s3-bucket](https://vinkius.com/mcp/amazon-s3-bucket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon S3 Bucket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amazon-s3-bucket` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon S3 Bucket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-s3-bucket": {
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
