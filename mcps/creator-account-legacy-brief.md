# Creator Account Legacy Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creator-account-legacy-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Consolidate digital assets, access protocols, and publishing mandates for creator estate planning.

## Description
This MCP server provides a specialized system for managing digital asset continuity. It allows AI agents to retrieve a complete overview of a creator's ecosystem, including platform inventories, content storage locations, collaborator matrices, and specific publishing or archiving mandates. Use `get_platform_inventory` to map the ecosystem, `list_content_locations` to find media, `resolve_collaborator_matrix` to identify stakeholders, and `audit_publishing_and_archive_plans` to execute transition instructions.


## Available Tools (4)
- **resolve_collaborator_matrix**: Maps the relationship between the creator, their collaborators, and their legal/professional authorized contacts
- **list_content_locations**: Locates where specific media assets and historical data are stored across the ecosystem
- **audit_publishing_and_archive_plans**: Retrieves the specific instructions regarding what happens to content upon a transition event
- **get_platform_inventory**: Identifies all digital platforms currently part of the creator's ecosystem


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creator Account Legacy Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all digital platforms for creator ID 'user_123'."

**🤖 AI Agent:**
> The platforms associated with creator 'user_123' are YouTube (Primary Hub), Instagram (Distribution Channel), and Gmail (Utility/Admin).

---

**👤 You:**
> "Where are the video files for 'creator_99' stored?"

**🤖 AI Agent:**
> Videos for 'creator_99' are stored in Cloud-based storage on YouTube and Local-hard-drive storage.

---

**👤 You:**
> "Who are the authorized contacts for 'creator_456'?"

**🤖 AI Agent:**
> The authorized contacts for 'creator_456' include Jane Doe (Legal Representative) and John Smith (Successor).


## ❓ FAQ

**Q: How can I see all platforms used by a creator?**
You can use the `get_platform_inventory` tool by providing the unique `creatorId` to retrieve a list of all associated platforms.

**Q: Can I find where specific videos are stored?**
Yes, use the `list_content_locations` tool. You can optionally filter by `contentCategory` such as 'video' to find specific storage types.

**Q: How do I know what to do with content after a transition?**
Use the `audit_publishing_and_archive_plans` tool. You must specify if you are auditing 'publishing_mandates' or 'archive_preferences'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creator-account-legacy-brief](https://vinkius.com/en/ai-agent-connect/creator-account-legacy-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creator Account Legacy Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creator-account-legacy-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creator Account Legacy Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creator-account-legacy-brief": {
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
