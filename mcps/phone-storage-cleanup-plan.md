# Phone Storage Cleanup Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/phone-storage-cleanup-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Analyze phone storage to identify space-saving opportunities and prioritize data management.

## Description
This MCP server provides tools to analyze phone storage data, helping users identify recoverable space and prioritize data management. Use `analyze_storage_usage` to get a high-level overview of storage distribution, `identify_removal_candidates` to find safe files for deletion, `list_backup_priority_items` to protect high-value data, and `get_app_footprint_details` to inspect specific application footprints.


## Available Tools (4)
- **get_app_footprint_details**: Drills down into the specific contents of a single application's storage
- **identify_removal_candidates**: Finds specific items that are safe and efficient to delete to free up space
- **list_backup_priority_items**: Identifies important data that must be backed up before any cleanup action is taken
- **analyze_storage_usage**: Provides a high-level overview of how storage is distributed across different categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phone Storage Cleanup Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my phone storage usage."

**🤖 AI Agent:**
> Your total storage is 128GB. The largest category is UserMedia at 45GB, followed by AppData at 30GB. You have 12GB of recoverable space.

---

**👤 You:**
> "What files can I delete to save space?"

**🤖 AI Agent:**
> You can free up 4.5GB by removing 12 old cache files and 2 large videos that have already been backed up.

---

**👤 You:**
> "How much space is the Photos app using?"

**🤖 AI Agent:**
> The Photos app is using 15.2GB of storage, consisting of 1,200 files including images and videos.


## ❓ FAQ

**Q: How can I see which apps are using the most space?**
You can use the `analyze_storage_usage` tool to view the app distribution and see which applications are consuming the most storage.

**Q: What files are safe to delete?**
The `identify_removal_candidates` tool identifies files that are marked as removable and meet your specific size or age criteria.

**Q: How do I know what to back up first?**
Use `list_backup_priority_items` to find high-value media or large, old files that should be secured before any cleanup occurs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/phone-storage-cleanup-plan](https://vinkius.com/en/ai-agent-connect/phone-storage-cleanup-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phone Storage Cleanup Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phone-storage-cleanup-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phone Storage Cleanup Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phone-storage-cleanup-plan": {
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
