# Personal Photos Archive Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-photos-archive-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media](../categories/media.md)

Organize photo collections with automated consent, storage, and preservation planning.

## Description
This MCP server provides a strategic planning system for photo archives. It manages the complexity of digital preservation by enforcing strict rules for consent, storage redundancy, and maintenance schedules. Use `plan_archive_structure` to define your folder hierarchy and storage mapping, `generate_access_matrix` to ensure privacy compliance, `calculate_preservation_schedule` to automate maintenance tasks, and `validate_storage_compliance` to audit your plan against the Primary-Copy and Backup-Location rules.


## Available Tools (4)
- **validate_storage_compliance**: Audits the proposed plan to ensure the Primary-Copy and Backup-Location rules are strictly followed
- **calculate_preservation_schedule**: Creates a recurring calendar of maintenance tasks (integrity checks and backup refreshes)
- **generate_access_matrix**: Determines who can see which albums based on the intersection of consent and group permissions
- **plan_archive_structure**: Generates the high-level organization of the archive, including the processing order and the physical/digital folder structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Photos Archive Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan an archive for my family photos from 1990-2000. John has granted consent, but Mary has restricted consent."

**🤖 AI Agent:**
> I have generated the archive structure. The 1990-2000 collection is prioritized as Legacy, and the access matrix has been restricted to ensure Mary's privacy is maintained.

---

**👤 You:**
> "Check if my current photo storage plan follows the backup rules."

**🤖 AI Agent:**
> The plan is compliant. All collections have a designated primary copy and at least one secondary backup location.

---

**👤 You:**
> "Create a maintenance schedule for my high-priority legacy photos."

**🤖 AI Agent:**
> The maintenance schedule is ready. High-priority legacy collections are scheduled for integrity checks every 6 months.


## ❓ FAQ

**Q: How does the system handle privacy?**
The system uses `generate_access_matrix` to cross-reference person consent status with group permissions, ensuring no unauthorized access to restricted photos.

**Q: What are the storage rules?**
The system enforces the Primary-Copy and Backup-Location rules. You can use `validate_storage_compliance` to verify that every collection has one primary copy and at least one secondary backup.

**Q: How often should I check my photo backups?**
Maintenance frequency is determined by priority. Use `calculate_preservation_schedule` to generate a custom calendar where Legacy collections are checked every 6 months.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-photos-archive-planner](https://vinkius.com/en/ai-agent-connect/personal-photos-archive-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Photos Archive Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-photos-archive-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Photos Archive Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-photos-archive-planner": {
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
