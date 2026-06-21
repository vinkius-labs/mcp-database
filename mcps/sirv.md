# Sirv MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sirv)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enable your AI agent to manage files, read metadata, and monitor bandwidth usage on your Sirv CDN account.

## Description
Connect your AI to **Sirv**, the image CDN and digital asset management platform optimized for speed and automation.

### What you can do

- **File Browsing** — List files and directories in your Sirv account, inspecting folder structures and contents.
- **Metadata Inspection** — Read detailed metadata for any file, including dimensions, format, size, and modification dates.
- **File Deletion** — Remove unused or outdated assets from your Sirv storage directly from chat.
- **Bandwidth Monitoring** — Audit your CDN bandwidth usage and storage consumption.

### How it works

1. Add the Sirv integration to your AI toolset.
2. Provide your Client ID and Client Secret.
3. Manage your media assets via natural language.

### Who is this for?

- **E-commerce Teams** — Audit product image libraries and clean up unused assets.
- **Web Developers** — Check file metadata and manage CDN content without opening the Sirv dashboard.
- **Content Managers** — Monitor storage usage and organize media assets from chat.


## Available Tools
- **delete_file**: This action is irreversible.

Permanently deletes a file
- **get_account_stats**: Retrieves Sirv account storage and traffic statistics
- **get_billing_info**: Retrieves billing details
- **get_file_details**: Retrieves details for a specific file
- **get_detailed_usage**: Retrieves detailed usage metrics
- **list_custom_domains**: Lists custom domains configured for the account
- **list_account_users**: Lists all users in the Sirv account
- **read_directory**: Requires the absolute path starting with "/".

Lists contents of a specific directory
- **search_files**: Returns file metadata and URLs.

Searches for files in Sirv


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sirv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the contents of the '/images' directory in my Sirv account."

**🤖 AI Agent:**
> Directory '/images' contains 15 items:
- 12 images (JPEG, PNG, WebP)
- 3 PDF documents
Total size: 48.2 MB. Would you like metadata details for any specific file?

---

**👤 You:**
> "Show me the bandwidth usage for this month."

**🤖 AI Agent:**
> Bandwidth usage for April 2026:
- Total transferred: 124.5 GB
- Storage used: 2.3 GB / 10 GB
- Requests: 1.2M
- Peak day: April 1 (18.3 GB)
You're at 62.3% of your monthly bandwidth allowance.


## ❓ FAQ

**Q: Can it accidentally delete all my files?**
The delete_file tool only removes the specific file you target by path. It cannot delete entire directories at once. Each deletion requires an explicit file path.

**Q: How does authentication work?**
You provide your Client ID and Client Secret. The integration automatically exchanges them for a Bearer token on each session — no manual OAuth setup required.

**Q: What file types does Sirv support?**
Sirv supports images (JPEG, PNG, WebP, SVG, GIF), videos, PDFs, and other static files. The integration can browse and manage all file types stored in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sirv](https://vinkius.com/mcp/sirv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sirv** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sirv` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sirv** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sirv": {
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
