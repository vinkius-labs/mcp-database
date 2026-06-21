# UPYUN Developer Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upyun-developer-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Bring UPYUN's Massive CDN and Image Processing APIs to your AI. Interact with buckets and deploy files to the cloud.

## Description
Integrate your AI with **UPYUN** (又拍云), one of the most prominent Cloud and CDN providers in the world. This MCP gives your agent direct file management access to your cloud buckets.

### What you can do

- **Cloud Storage Management** — Automatically create, view, list, and delete files inside your UPYUN buckets without downloading their manual command line clients
- **CDN Artifact Uploads** — Enable the LLM to directly write code logic or textual artifacts and deploy them live to your CDN domains instantly
- **Capacity Auditing** — Fetch storage usage to monitor consumption on your buckets dynamically

### How it works

1. Subscribe to this server
2. Obtain an Operator Name and Password inside your bucket's API access page
3. Plug the credentials into your agent and you are fully connected. The MCP abstracts away the legacy HMAC-SHA1 Authorization header generation securely.

### Who is this for?

- **DevOps Agents** — Automate static site generation and deployments directly pushing file changes to UPYUN instances
- **Frontend Engineers** — Skip writing complex Python deploy scripts when prototyping web applications
- **Content Administrators** — Check what is currently inside specific UPYUN directories via natural language


## Available Tools
- **create_text_file**: Create and upload a text file directly to UPYUN
- **delete_file**: Delete a file from UPYUN
- **get_file_info**: Get metadata about an UPYUN file
- **get_service_usage**: Get UPYUN bucket service usage
- **list_directory**: g., "/" or "/images/") to list its contents.

List files and folders in an UPYUN directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UPYUN Developer Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files present in the root `/` directory of my Upyun bucket."

**🤖 AI Agent:**
> Here is the directory listing for your root path. It contains 3 folders (`images/`, `assets/`, `scripts/`) and 2 files (`index.html`, `style.css`).

---

**👤 You:**
> "Create a new text file at `/hello.txt` with the content 'Hello from MCP'."

**🤖 AI Agent:**
> I've successfully created the file `/hello.txt` in your UPYUN bucket and uploaded the text string you requested.


## ❓ FAQ

**Q: Where do I find my UPYUN Operator details?**
Log into your UPYUN console, click on 'Cloud Storage' -> 'Your Service/Bucket' -> 'Configuration' -> 'Operators'. From there you can copy the operator name and the generated password.

**Q: Does the AI see my files if I connect this?**
The AI uses this MCP to only perform the standard API queries you allow it. Use an Operator with specific folder limits if you wish to restrict directory access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upyun-developer-platform](https://vinkius.com/mcp/upyun-developer-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UPYUN Developer Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `upyun-developer-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UPYUN Developer Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upyun-developer-platform": {
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
