# Download Folder Cleanup Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/download-folder-cleanup-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [storage](../categories/storage.md)

Analyze and organize download history to identify duplicates, space usage, and archive candidates.

## Description
This MCP server provides tools to analyze your download directory and create actionable cleanup strategies. Use `calculate_space_by_category` to see which file types consume the most storage, `identify_duplicates` to find bit-for-bit identical files, and `propose_archive_groups` to bundle old files for long-term storage. You can also use `get_review_folders` to group files by extension, year, or size for easier inspection.


## Available Tools (4)
- **get_review_folders**: Identifies logical groupings of files that require user intervention based on specific criteria
- **calculate_space_by_category**: ) are taking up the most space.

Summarizes how much disk space is being consumed by different file types
- **identify_duplicates**: Finds groups of files that are exact bit-for-bit copies of one another
- **propose_archive_groups**: Suggests bundles of files that can be moved to an archive based on age and type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Download Folder Cleanup Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much space is my media folder taking up?"

**🤖 AI Agent:**
> Your Media category is currently consuming 4.2 GB of space across 12 files.

---

**👤 You:**
> "Find all my duplicate files."

**🤖 AI Agent:**
> I found 3 groups of exact duplicates consisting of 5 files in total.

---

**👤 You:**
> "Suggest some files I can archive that are older than 30 days."

**🤖 AI Agent:**
> I suggest the following archive group: 'Old Documents from 2023' containing 'report_v1.pdf' and 'notes_old.txt'.


## ❓ FAQ

**Q: How does the tool handle files I want to keep?**
Files marked with a 'keep' flag are excluded from duplicate detection and archive proposals to ensure your essential files are never suggested for deletion.

**Q: Can I group files by their file extension?**
Yes, you can use `get_review_folders` with the 'extension' grouping parameter to see files organized by their type.

**Q: What is an archive group?**
An archive group is a logical bundle of old files suggested by `propose_archive_groups` that can be moved to long-term storage in a single action.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/download-folder-cleanup-plan](https://vinkius.com/en/ai-agent-connect/download-folder-cleanup-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Download Folder Cleanup Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `download-folder-cleanup-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Download Folder Cleanup Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "download-folder-cleanup-plan": {
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
