# FlowUs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

All-in-one knowledge management and collaboration platform — manage pages, blocks, and databases via AI.

## Description
Empower your AI agent to orchestrate your knowledge base with **FlowUs**, the versatile collaboration platform for modern individuals and teams. By connecting FlowUs to your agent, you transform complex page organization and database management into a natural conversation. Your agent can instantly list your pages, retrieve block-level content, manage multi-dimensional databases, and even create new entries without you needing to navigate the complex web interface. Whether you are managing personal notes, project documentation, or shared team databases, your agent acts as a real-time knowledge assistant, keeping your workspace organized and your information accessible.

### What you can do

- **Page Orchestration** — List all accessible pages and retrieve detailed metadata about your workspace structure.
- **Block Management** — Browse content blocks within pages to access text and media information instantly.
- **Database Control** — Manage multi-dimensional tables (databases) with full support for querying and creating new rows.
- **Workspace Organization** — Create and update pages to maintain a clean and structured knowledge base.
- **Team Coordination** — Access workspace user lists to manage participation and collaboration effectively.

### How it works

1. Subscribe to this server
2. Enter your FlowUs API Token
3. Start managing your knowledge base through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — automate note-taking and organize project documentation through natural language.
- **Product Managers** — track feature requirements and manage product roadmaps directly from your AI-powered workspace.
- **Operations Teams** — oversee shared databases and team wikis through a unified AI interface.
- **Students & Researchers** — manage study notes and research databases without manual technical overhead.


## Available Tools
- **create_database_row**: Add row to database
- **create_page**: Create a new FlowUs page
- **get_database**: Get database schema
- **get_page**: Get page details
- **list_blocks**: ) within a specific page.

List page blocks
- **list_databases**: List all FlowUs databases
- **list_pages**: List all FlowUs pages
- **list_users**: List workspace users
- **query_database**: Query database rows
- **update_page**: Update an existing page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FlowUs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pages in my FlowUs workspace."

**🤖 AI Agent:**
> I've retrieved your FlowUs pages. You have 6 active pages, including 'Project Roadmap' and 'Meeting Notes'. Which one would you like to view the content for?

---

**👤 You:**
> "Query the 'Product Backlog' database for items with 'High' priority."

**🤖 AI Agent:**
> I've queried the 'Product Backlog' database. I found 3 items with high priority: 'Refactor Auth Engine', 'Implement PDF Export', and 'API Documentation'. Would you like more details on any of them?

---

**👤 You:**
> "Add a new row to the 'User Feedback' database with Name='Renato' and Feedback='Love the AI integration!'."

**🤖 AI Agent:**
> Done! I've added your feedback to the 'User Feedback' database. The new entry for Renato has been successfully created.


## ❓ FAQ

**Q: How do I find my FlowUs API Token?**
Log in to FlowUs, go to [Settings] → [Integrations] → [Bot Integrations], and create a new integration to generate your API Token.

**Q: Can I search for specific data within a database?**
Yes. Use the `query_database` tool with the database ID. You can optionally provide a JSON filter string to narrow down the results based on your criteria.

**Q: What is a 'Block' in FlowUs?**
Like Notion, FlowUs uses a block-based structure. Everything from a paragraph of text to an image or a sub-page is considered a block. You can list these using the `list_blocks` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowus](https://vinkius.com/mcp/flowus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FlowUs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flowus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FlowUs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flowus": {
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
