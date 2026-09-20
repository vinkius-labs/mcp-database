# Microsoft OneDrive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/microsoft-onedrive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Browse, search, upload, share, and manage OneDrive files through one connected drive — your cloud folder for any AI agent.

## Description
Give any AI agent a working file cabinet on your **OneDrive** drive. Through the Microsoft Graph API the agent can walk folders, find files by keyword, read file metadata, prepare uploads, and build share links — all inside your personal or OneDrive for Business drive.

### What you can do

- **Browse & Inspect** — List any folder newest-first, drill into subfolders, and pull metadata (size, creator, last modifier, web URL) for a specific item
- **Find Anything** — Full-drive keyword search with ordered results, plus a recent-activity feed for "what was I doing" moments
- **Bring Files In** — Upload base64 content to an exact folder path, with folder scaffolding before the drop
- **Share Safely** — Create read or resolve permissions and hand the agent-generated link to anyone

### How it works

1. Register an Entra application with Microsoft Graph Files.Read / Files.ReadWrite delegated permissions
2. Subscribe to this server and connect your OneDrive account through OAuth 2.0
3. Point the agent at your drive and let it navigate, search, and share for you

### Who is this for?

- **Consultants & Operators** — drop deliverables into a client folder and generate share links without leaving the chat
- **Knowledge Workers** — keep documents, reports, and reference files one natural-language command away


## Available Tools (8)
- **create_folder**: Use to prepare a structure before uploading files. An already-existing folder produces an item-already-exists error — treat that as success and continue.

Create a folder in OneDrive
- **download_file**: Use when the user wants to fetch or open a binary from OneDrive. Large or protected files may fail — if so, report the link error instead of retrying blindly.

Get a direct download link for a OneDrive file
- **get_file**: Use when the user asks about a specific file that list_files or search_files located. Paths are relative to the drive root, e.g. "Reports/2026/Q3.xlsx".

Get metadata for a specific OneDrive file or folder
- **list_files**: Use when the user wants to browse their OneDrive. An empty path means the drive root. Page large folders with top and skip — results are one page at a time.

List files and folders in a OneDrive directory
- **recent_files**: Use for "what was I working on" style questions without knowing folder locations. Page with top when the user wants more than the default batch.

List recently active items on the OneDrive drive
- **search_files**: Use when the user is looking for something but does not know its exact folder. The query matches file names and content; combine with top to cap results.

Search the entire OneDrive drive by keyword
- **share_file**: Use when the user wants to share something with others. Default role is read; use resolve when recipients need to open it in OneDrive. Anonymous links may be blocked by tenant policy — report that clearly if sharing fails.

Create a share permission for a OneDrive file or folder
- **upload_file**: Use when the agent already holds small file bytes (under about 100 MB) and needs to store them. The parent path must exist; create it with create_folder first if unsure.

Upload a file to OneDrive from base64 content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft OneDrive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What files did I touch this week? Give me the five most recently modified documents."

**🤖 AI Agent:**
> Here are your five most recent: Q3-Forecast.xlsx (Mon 18:42), Client-Redline.docx (Mon 09:10), deck-v7.pptx (Sun 21:03), invoices-08.csv (Fri 16:20), notes.txt (Fri 11:05). Want me to open or share any of them?

---

**👤 You:**
> "Create a 'Client Acme / 2026' folder structure and upload the contract PDF I just generated."

**🤖 AI Agent:**
> Folders 'Client Acme' and 'Client Acme/2026' are in place, and Acme-Contract-v2.pdf (412 KB) is now in that folder. I can drop a read-only share link in the thread if you want.

---

**👤 You:**
> "Find every file that mentions 'renewal' in its name and share a read link with our account manager."

**🤖 AI Agent:**
> Three matches: Renewal-Plan-2026.xlsx, client-renewal-notes.docx, and renewal-emails-export.csv. Share links created (read role) — links added to this thread. Note: the CSV is 1.2 MB, fine for a link, but I would not inline it.


## ❓ FAQ

**Q: Does it work with both personal OneDrive and OneDrive for Business?**
Yes. The Graph /me/drive resource resolves to whichever drive belongs to the connected account — personal Microsoft accounts and work or school (Business) tenants both work through the same OAuth flow.

**Q: Can the agent read the actual contents of a document?**
It retrieves metadata and a short-lived direct download URL. For text analysis, hand that URL to a document-parsing tool or download step in your pipeline — the drive server itself does not proxy file bytes.

**Q: What happens if I share a file with anonymous links blocked in my tenant?**
The permission call fails with a tenant policy error and the tool surfaces it verbatim. Try the resolve role or have an admin adjust the external sharing policy; the agent will not loop on retries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/microsoft-onedrive](https://vinkius.com/en/ai-agent-connect/microsoft-onedrive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft OneDrive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microsoft-onedrive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft OneDrive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-onedrive": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
