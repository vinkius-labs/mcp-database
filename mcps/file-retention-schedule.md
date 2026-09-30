# File Retention Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/file-retention-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document lifecycle management by calculating keep, archive, review, and deletion dates.

## Description
Manage the lifecycle of digital documents with precision. This MCP server connects AI agents to regulatory and organizational retention rules, allowing them to determine exactly when files should be kept, archived, reviewed, or destroyed. Use `calculate_retention_milestones` to generate full timelines for specific files, or `filter_files_by_action` to identify batches of documents ready for the next lifecycle stage. It ensures compliance by validating retention overrides and retrieving category-specific rules.


## Available Tools (4)
- **calculate_retention_milestones**: Calculates the full lifecycle timeline for a specific file based on its metadata and retention rules
- **filter_files_by_action**: Identifies a list of files that have reached a specific lifecycle stage
- **get_category_rules**: Retrieves the default retention settings for a specific document classification
- **validate_retention_override**: Verifies if a user-provided retention override is compliant with organizational policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **File Retention Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the lifecycle timeline for file ID 'doc_123' which is a 'Tax' document created on 2020-01-01?"

**🤖 AI Agent:**
> For file doc_123 (Tax), the keep date is 2030-01-01, the archive date is 2025-01-01, the review date is 2029-01-01, and the delete-on date is 2030-01-01.

---

**👤 You:**
> "Are there any files ready to be deleted as of today?"

**🤖 AI Agent:**
> There are 12 files currently eligible for permanent destruction based on their retention schedules.

---

**👤 You:**
> "What are the default retention rules for the 'HR' category?"

**🤖 AI Agent:**
> The default retention for HR documents is 5 years, with archiving occurring after 3 years and a review triggered 1 year before deletion.


## ❓ FAQ

**Q: How does a legal hold affect file retention?**
When a legal hold is active, the `calculate_retention_milestones` tool ensures the deletion date is pushed to the infinite future, preventing any files from being flagged for destruction.

**Q: Can I override the default retention period for a category?**
You can attempt an override, but you should first use `validate_retention_override` to ensure the proposed duration complies with mandatory regulatory requirements for that category.

**Q: How can I find all files that need to be archived?**
You can use the `filter_files_by_action` tool with the 'archive' action type and a specific reference date to retrieve a list of all files ready for long-term storage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/file-retention-schedule](https://vinkius.com/en/ai-agent-connect/file-retention-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **File Retention Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `file-retention-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **File Retention Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "file-retention-schedule": {
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
