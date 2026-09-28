# Personal Archive Migration Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-archive-migration-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Converts chaotic data inventories into structured, secure migration schedules.

## Description
This MCP server provides a specialized planning engine for digital data migrations. It transforms disorganized file inventories into actionable migration schedules, complete with folder mapping, security-aware checkpoint plans, and verification checklists. Use `plan_migration_schedule` to establish timelines, `map_folder_structure` to define destination paths, `generate_checkpoint_plan` to ensure data integrity based on sensitivity tiers, and `build_verification_checklist` to confirm successful transfers.


## Available Tools (4)
- **build_verification_checklist**: Produces a list of tasks to validate that the migration was successful
- **generate_checkpoint_plan**: Identifies optimal moments during the migration to pause and verify data integrity
- **map_folder_structure**: Creates a blueprint of where every source file will live in the new destination
- **plan_migration_schedule**: Generates a chronological timeline for moving data from source to destination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Archive Migration Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a migration schedule for 500 files with a deadline of 2025-12-31 and a limit of 50 files per batch."

**🤖 AI Agent:**
> I have generated a migration schedule consisting of 10 batches, each containing 50 files, scheduled to be completed well before the December 31st, 2025 deadline.

---

**👤 You:**
> "Map these files to my new taxonomy: ['/photos/img1.jpg', '/docs/file1.pdf'] using the structure {'Photos': 'Archive/Images', 'Docs': 'Archive/Documents'}."

**🤖 AI Agent:**
> The files have been mapped: '/photos/img1.jpg' will move to 'Archive/Images/img1.jpg' and '/docs/file1.pdf' will move to 'Archive/Documents/file1.pdf'.

---

**👤 You:**
> "Generate a verification checklist for my migration."

**🤖 AI Agent:**
> The verification checklist is ready. It includes a total file count comparison between source and destination and a structural integrity check of the folder hierarchy.


## ❓ FAQ

**Q: How do I create a timeline for my data move?**
You can use the `plan_migration_schedule` tool by providing your file inventory, the target deadline, and your preferred batch constraints.

**Q: How does the tool handle sensitive data?**
The engine uses `generate_checkpoint_plan` to automatically insert verification pauses after any batch containing Restricted or High sensitivity data.

**Q: Can I avoid moving duplicate files?**
Yes, by using the `map_folder_structure` tool and providing a list of duplicate identifiers, the engine will exclude them from the final destination map.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-archive-migration-planner](https://vinkius.com/en/ai-agent-connect/personal-archive-migration-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Archive Migration Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-archive-migration-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Archive Migration Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-archive-migration-planner": {
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
