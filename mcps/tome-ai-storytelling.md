# Tome (AI Storytelling) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tome-ai-storytelling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate and manage AI-powered presentations via Tome — list workspaces, manage tomes, and add pages directly from any AI agent.

## Description
Connect your **Tome** account to any AI agent to streamline your AI-driven storytelling and presentation workflows through natural conversation.

### What you can do

- **Workspaces & Tomes** — List all accessible workspaces and fetch active tomes directly from the Tome cloud
- **Tome Management** — Create new tomes in specific workspaces and organize your storytelling projects
- **Page Operations** — Add new pages to existing tomes to expand your narrative dynamically
- **Deep Inspection** — Fetch complete metadata and page details for specific tomes to understand their structure

### How it works

1. Subscribe to this server
2. Enter your Tome API Key
3. Start generating presentations from Claude, Cursor, or any MCP-compatible client

No more manual slide creation. Your AI acts as a creative director, building out your vision page by page.

### Who is this for?

- **Content Creators** — instantly scaffold stories and presentations without leaving your AI chat
- **Marketing Teams** — manage workspace assets and create new campaign decks via automation
- **Product Managers** — document features and roadmaps by generating tomes directly from project specs


## Available Tools
- **add_page**: Add a new page to an existing tome
- **create_tome**: Create a new tome in a workspace
- **get_tome**: Get detailed information about a specific tome
- **list_tomes**: List tomes in a workspace
- **list_workspaces**: List Tome workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tome (AI Storytelling)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Tome workspaces."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have access to: 'Personal Space' (ID: ws_987) and 'Design Team' (ID: ws_654). Which one would you like to explore?

---

**👤 You:**
> "Create a new tome titled 'Product Roadmap 2025' in workspace ws_987."

**🤖 AI Agent:**
> Successfully created! Your new tome 'Product Roadmap 2025' is now live in your Personal Space with ID: tome_abc123. Would you like to add the first page?

---

**👤 You:**
> "Add a page called 'Market Analysis' to tome tome_abc123."

**🤖 AI Agent:**
> Done. I've added the 'Market Analysis' page to your tome. You can now see it in the presentation structure.


## ❓ FAQ

**Q: Can I see the full structure of a specific presentation including its pages?**
Yes! Use the `get_tome` tool with the specific Tome ID. Your agent will retrieve detailed information about the tome, including its page list and metadata.

**Q: How do I add a new slide or page to an existing project?**
Simply use the `add_page` action. Provide the `tome_id` and the `title` for your new page, and the agent will insert it into your presentation immediately.

**Q: Can I list all the presentations I have in a specific workspace?**
Yes, use the `list_tomes` tool. By providing the `workspace_id`, the agent will return a list of all tomes available in that specific environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tome-ai-storytelling](https://vinkius.com/mcp/tome-ai-storytelling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tome (AI Storytelling)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tome-ai-storytelling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tome (AI Storytelling)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tome-ai-storytelling": {
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
