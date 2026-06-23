# Google Cloud Storage Bucket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-storage-bucket)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages files in a single Google Cloud Storage Bucket. That's its only function, and nothing else. Incredible for giving your AI secure file storage.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to read, write, and list files inside one specific GCS Bucket.**

By strictly scoping access, your AI can safely persist data, analyze documents, and manage its own workload without ever touching your critical cloud infrastructure.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single bucket. It cannot list other buckets or delete your company's production backups.
- **Native GCP Integration:** Direct, high-performance interactions with Google Cloud using Service Account credentials.
- **Plug & Play File System:** Instantly gives your agent a massive cloud hard drive to store its memories, generated assets, and processed reports.


## Available Tools (4)
- **delete_object**: Delete an object from the Google Cloud Storage bucket
- **get_object**: Read the content of an object in the Google Cloud Storage bucket
- **list_objects**: List objects in the configured Google Cloud Storage bucket
- **put_object**: If the object already exists, it is overwritten.

Upload or overwrite an object in the Google Cloud Storage bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Storage Bucket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files inside the 'data/exports/' folder."

**🤖 AI Agent:**
> I found 3 files with the prefix 'data/exports/': export-1.csv, export-2.csv, and summary.json.

---

**👤 You:**
> "Upload this JSON configuration to 'configs/agent-settings.json'."

**🤖 AI Agent:**
> I've successfully uploaded the JSON data to 'configs/agent-settings.json' with `content-type: application/json`.

---

**👤 You:**
> "Delete the temporary 'processing/job-123.tmp' file."

**🤖 AI Agent:**
> The file 'processing/job-123.tmp' was successfully deleted from the Google Cloud Storage bucket.


## ❓ FAQ

**Q: Why limit the agent to a single GCS Bucket?**
To enforce zero-trust security. An autonomous AI agent should never have carte blanche to read or delete objects across your entire Google Cloud project.

**Q: How does the Service Account authentication work?**
The MCP uses the Project ID, Client Email, and Private Key from your GCP Service Account JSON to sign JWT tokens and seamlessly access the GCS REST API.

**Q: Can it read binary files?**
Currently, the tool returns the raw text content. If you download a binary image, it will be represented as a raw string. It is best used for JSON, Markdown, CSVs, or logs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-storage-bucket](https://vinkius.com/mcp/google-cloud-storage-bucket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Cloud Storage Bucket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-cloud-storage-bucket` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Cloud Storage Bucket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-cloud-storage-bucket": {
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
