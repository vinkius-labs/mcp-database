# Photo Library Deduplication Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-library-deduplication-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [storage](../categories/storage.md)

Identify and resolve redundant photo records by analyzing technical metadata.

## Description
This MCP server provides tools to manage digital photo libraries by identifying exact duplicates. Using technical metadata like file hashes, capture times, and dimensions, it can find redundant files and calculate recoverable storage space. It includes deterministic logic to select the best master file to keep and safety checks to prevent accidental data loss of unique images. Use `find_duplicate_groups` to locate duplicates and `analyze_recovery_impact` to see how much space you can save.


## Available Tools (4)
- **analyze_recovery_impact**: Calculate the total storage impact of a deduplication plan
- **find_duplicate_groups**: Identify sets of photo records that are considered exact duplicates
- **select_master_files**: Determine which specific file should be kept for every identified duplicate group
- **validate_deduplication_safety**: Verify that a proposed deduplication plan will not result in data loss of unique files


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Library Deduplication Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all duplicate photo groups in this list: [{'hash': 'abc123', 'captureTime': '2023-01-01T12:00:00Z', 'dimensions': '4000x3000', 'size': 5000000, 'storagePath': '/photos/img1.jpg'}, {'hash': 'abc123', 'captureTime': '2023-01-01T12:00:00Z', 'dimensions': '4000x3000', 'size': 5000000, 'storagePath': '/photos/copy_img1.jpg'}]"

**🤖 AI Agent:**
> { "groups": [{ "masterFile": { "hash": "abc123", "captureTime": "2023-01-01T12:00:00Z", "dimensions": "4000x3000", "size": 5000000, "storagePath": "/photos/img1.jpg" }, "duplicates": [{ "hash": "abc123", "captureTime": "2023-01-01T12:00:00Z", "dimensions": "4000x3000", "size": 5000000, "storagePath": "/photos/copy_img1.jpg" }], "recoverableBytes": 5000000 }] }

---

**👤 You:**
> "How much space can I recover from these duplicate groups?"

**🤖 AI Agent:**
> You can recover a total of 5,000,000 bytes by deleting the redundant files.

---

**👤 You:**
> "Which file should I keep for the duplicate group with hash 'xyz789'?"

**🤖 AI Agent:**
> The file at '/photos/img_main.jpg' should be kept as the master file.


## ❓ FAQ

**Q: How does the system identify a duplicate?**
A photo is considered an exact duplicate if it shares the same file hash, capture time, and dimensions.

**Q: How is the master file chosen?**
The system uses deterministic rules: it prioritizes the file with the shortest storage path. If paths are equal, it selects the one with the most recent timestamp.

**Q: Is it safe to run the deduplication plan?**
Yes, you can use `validate_deduplication_safety` to verify that the proposed deletions will not result in the loss of any unique files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-library-deduplication-plan](https://vinkius.com/en/ai-agent-connect/photo-library-deduplication-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Library Deduplication Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-library-deduplication-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Library Deduplication Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-library-deduplication-plan": {
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
