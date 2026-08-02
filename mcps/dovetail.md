# Dovetail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dovetail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze qualitative research data with AI-powered tagging, theme discovery, and insight synthesis for product and UX teams.

## Description
Connect your **Dovetail** account to any AI agent and take full control of your user research and insight management workflows through natural conversation.

### What you can do

- **Project Orchestration** — List and manage research projects programmatically and retrieve detailed metadata about goals and participants
- **Note Architecture** — Create and organize research notes (interviews, usability tests, raw data) with specific content types (HTML, Markdown) directly from your agent
- **Insight Management** — Programmatically publish research findings and summaries to maintain a high-fidelity record of your team's discoveries
- **Deep Search** — Find relevant research data across projects using powerful query filters for titles and content
- **Workspace Visibility** — Retrieve complete directories of workspace members to coordinate collaboration and manage team access

### How it works

1. Subscribe to this server
2. Retrieve your **Personal API Key** from Dovetail settings (Settings > Account > Personal API keys)
3. Start managing your research data from Claude, Cursor, or any MCP client

No more manual scrubbing through interview transcripts or complex project navigation. Your AI acts as your dedicated user research and insight coordinator.

### Who is this for?

- **User Researchers** — instantly register new interview notes and publish highlights using natural language commands
- **Product Managers** — search across research projects to find specific user pain points and insights without leaving your workspace
- **Design Leads** — monitor research progress and manage team collaboration through simple AI queries


## Available Tools (7)
- **create_insight**: Create a new research insight
- **create_note**: Create a new research note
- **get_project_details**: Get details for a research project
- **list_insights**: List research insights
- **list_notes**: List research notes
- **list_projects**: List all research projects
- **list_workspace_members**: List workspace members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dovetail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my research projects in Dovetail."

**🤖 AI Agent:**
> I've retrieved your research projects. You have 3 active studies, including 'Mobile UX Redesign' (ID: proj_123) and 'Q4 User Feedback'. Which one would you like to inspect for notes?

---

**👤 You:**
> "Create a new research note 'User A Interview' in project 'proj_123'."

**🤖 AI Agent:**
> Note created! 'User A Interview' is now added to the Mobile UX project (ID: proj_123). I've set the content type to HTML. Shall I add some initial highlights to this note?

---

**👤 You:**
> "Show me all published insights containing the word 'mobile'."

**🤖 AI Agent:**
> Searching insights... I've found 2 published findings related to 'mobile'. The most relevant is 'Mobile-first navigation trends' from the latest study. Would you like the full summary for this insight?


## ❓ FAQ

**Q: How do I find my Dovetail API Key?**
Log in to Dovetail, navigate to **Settings** > **Account** > **Personal API keys**, and generate a new key for your integration.

**Q: Can I search for specific notes across projects?**
Yes! Use the `list_notes` tool and provide a search term or specific project IDs in the `filter_json` parameter to narrow your results.

**Q: What content types are supported for notes?**
Notes support text/html, text/markdown, and text/plain. HTML is the default and recommended type for rich formatting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dovetail](https://vinkius.com/mcp/dovetail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dovetail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dovetail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dovetail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dovetail": {
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
