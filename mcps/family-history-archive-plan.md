# Family History Archive Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-history-archive-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic planning engine for organizing family history, oral histories, and digital archives.

## Description
This MCP server provides a suite of tools to transform raw family data into organized historical archives. Use `get_collection_plan` to create a roadmap for gathering assets, `generate_interview_schedule` to organize oral history sessions, `build_archive_structure` to create a logical folder hierarchy, and `map_sharing_permissions` to manage access based on individual consent. It is designed to maintain historical integrity through strict source attribution and preservation rules.


## Available Tools (4)
- **build_archive_structure**: Organizes the proposed archive into a logical, navigable hierarchy
- **generate_interview_schedule**: Creates a structured calendar of oral history sessions
- **get_collection_plan**: Generates a comprehensive roadmap for gathering all identified family assets
- **map_sharing_permissions**: Produces a security and access map based on individual consent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family History Archive Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan my collection. I have three relatives (John, Mary, and Alice) and I want to collect photos and letters over the next three months."

**🤖 AI Agent:**
> I have generated a collection plan. Your priority items are the letters from Alice, and your first step is to contact John to verify photo availability.

---

**👤 You:**
> "I need to schedule interviews with my grandfather about our family's migration story. He is available on weekends in October."

**🤖 AI Agent:**
> I have scheduled three interview sessions for the Saturdays in October, focusing on the migration story and early settlement details.

---

**👤 You:**
> "Organize these assets into a folder structure: 10 digital photos from 1950, 5 scanned letters from 1920, and 2 audio recordings of oral histories."

**🤖 AI Agent:**
> The archive will be organized into branches by era: a '1920s' folder for the letters and a '1950s' folder for the photos, with a dedicated 'Oral Histories' folder for the audio recordings.


## ❓ FAQ

**Q: How do I start a new family archive project?**
You can start by using `get_collection_plan` to define your roadmap once you have a list of relatives and assets to collect.

**Q: Can I manage privacy for sensitive family documents?**
Yes, use `map_sharing_permissions` to create a security map that respects the consent levels provided by each family member.

**Q: How are interview sessions organized?**
The `generate_interview_schedule` tool creates a structured calendar based on the availability of your interviewees and the topics you wish to cover.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-history-archive-plan](https://vinkius.com/en/ai-agent-connect/family-history-archive-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family History Archive Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-history-archive-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family History Archive Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-history-archive-plan": {
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
