# Scribe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scribe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create step-by-step guides and SOPs automatically by recording your workflow and generating visual documentation instantly.

## Description
Connect your **Scribe** organization to any AI agent and access your process documentation library through natural conversation.

### What you can do

- **Full Search** — Search across all Scribes and Knowledge Pages simultaneously.
- **Filtered Search** — Search only guides or only pages for targeted results.
- **Team Scoping** — Find documents within a specific team for departmental queries.
- **Date Filtering** — Search by creation date range or get recent documents.
- **Teams** — List all teams and their documents for content auditing.
- **Statistics** — Get an overview of your documentation footprint.

### How it works

1. Subscribe to this server
2. Enter your Scribe API key (Enterprise Grid or Global plan required)
3. Start searching documentation from Claude, Cursor, or any MCP client

### Who is this for?

- **Knowledge Managers** — quickly find and audit process documentation.
- **Support Teams** — retrieve step-by-step guides for customer assistance.
- **Operations Leads** — monitor documentation activity across teams.


## Available Tools (10)
- **check_scribe_status**: Verify Scribe API connectivity
- **get_documentation_stats**: Get documentation statistics
- **get_team_documents**: Useful for auditing team documentation.

Get all documents for a specific team
- **list_teams**: List all teams in your Scribe organization
- **search_documents**: Search across all Scribes and Pages
- **search_by_date**: Dates should be in YYYY-MM-DD format.

Search documents by creation date range
- **search_by_team**: Search documents within a specific team
- **search_pages**: Search only Knowledge Pages
- **get_recent_documents**: Get documents created in the last 30 days
- **search_scribes**: Search only Scribe guides


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scribe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all documentation about 'onboarding'."

**🤖 AI Agent:**
> Found 12 documents matching 'onboarding': 8 Scribe guides and 4 Knowledge Pages. The most relevant is 'New Employee Onboarding Checklist' (Scribe, HR team).

---

**👤 You:**
> "List all teams in our Scribe organization."

**🤖 AI Agent:**
> Your Scribe organization has 5 teams: Engineering (42 docs), Sales (28 docs), HR (19 docs), Marketing (15 docs), and Customer Support (31 docs).

---

**👤 You:**
> "What documents were created in the last 30 days?"

**🤖 AI Agent:**
> 7 documents were created in the last 30 days: 4 Scribes including 'API Integration Guide' and 'Deployment Checklist', plus 3 Knowledge Pages.


## ❓ FAQ

**Q: Can I search only for step-by-step guides?**
Yes! Use `search_scribes` to search exclusively for Scribe guides, or `search_pages` for Knowledge Pages only.

**Q: Do I need an Enterprise plan to use this?**
Yes, the Scribe Search & Retrieval API is available on Enterprise Grid and Global plans. Contact Scribe sales for API access.

**Q: Can I find documents by a specific team?**
Yes! First use `list_teams` to see available teams and their IDs, then use `search_by_team` or `get_team_documents` with the team ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scribe](https://vinkius.com/mcp/scribe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scribe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scribe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scribe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scribe": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
