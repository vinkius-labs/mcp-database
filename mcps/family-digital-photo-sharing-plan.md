# Family Digital Photo Sharing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-digital-photo-sharing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media](../categories/media.md)

Coordinate digital photo distribution, access rights, and family sharing calendars.

## Description
This MCP server acts as a coordination engine for managing digital photo distribution and access rights within a family ecosystem. It allows AI agents to manage album lifecycles using `get_album_workflow`, organize relatives via `get_access_groups`, verify contributor rights with `validate_upload_permission`, and schedule photo-gathering windows using `get_family_sharing_calendar`.


## Available Tools (4)
- **get_family_sharing_calendar**: Provides a schedule of upcoming photo-related events and their associated sharing windows
- **validate_upload_permission**: Checks if a specific relative has the right to contribute photos to a specific album
- **get_access_groups**: Retrieves the logical groupings of relatives to facilitate mass permission updates
- **get_album_workflow**: Determines the operational steps and rules required to manage a specific photo collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Digital Photo Sharing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the workflow for the 'Summer Vacation 2024' album?"

**🤖 AI Agent:**
> The workflow for the Summer Vacation 2024 album includes: 1. Collection, 2. Review, 3. Archiving. The primary owner is Sarah, and the retention policy is 5 years.

---

**👤 You:**
> "Can Uncle Bob upload photos to the 'Christmas 2023' album?"

**🤖 AI Agent:**
> No, Uncle Bob does not have permission to upload to the Christmas 2023 album.

---

**👤 You:**
> "Show me the photo sharing events between 2024-01-01 and 2024-12-31."

**🤖 AI Agent:**
> There are two events: 'Spring Reunion' on 2024-04-15 (Sharing window active) and 'Family Picnic' on 2024-07-20 (Sharing window closed).


## ❓ FAQ

**Q: How can I check if a relative can upload photos to an album?**
You can use the `validate_upload_permission` tool to check if a specific relative has the rights to contribute to a target album.

**Q: Can I see upcoming family events for photo sharing?**
Yes, the `get_family_sharing_calendar` tool provides a schedule of upcoming events and their active sharing windows.

**Q: How do I find all members in a specific family group?**
Use the `get_access_groups` tool to retrieve the list of members belonging to a specific access group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-digital-photo-sharing-plan](https://vinkius.com/en/ai-agent-connect/family-digital-photo-sharing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Digital Photo Sharing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-digital-photo-sharing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Digital Photo Sharing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-digital-photo-sharing-plan": {
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
