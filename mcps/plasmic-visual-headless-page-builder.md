# Plasmic (Visual Headless Page Builder) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plasmic-visual-headless-page-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Plasmic projects, pages, and components via AI — list projects, inspect page structures, and trigger publishes directly.

## Description
Connect your **Plasmic** visual headless page builder to any AI agent and take full control of your web projects through natural conversation.

### What you can do

- **Project Discovery** — List all your Plasmic projects and retrieve their unique IDs and metadata directly from the Studio.
- **Page Management** — Fetch all pages within a specific project to understand your site structure and routing.
- **Deployment** — Trigger project publishes directly from the chat to update your live site or headless storefront instantly.
- **Visual CMS Control** — Inspect project details and configurations without leaving your AI interface or code editor.

### How it works

1. Subscribe to this server
2. Enter your Plasmic Project ID and API Token
3. Start managing your visual projects from Claude, Cursor, or any MCP-compatible client

No more switching between the Plasmic Studio and your terminal to check project IDs or trigger builds. Your AI acts as a bridge to your visual development workflow.

### Who is this for?

- **Developers** — quickly check page structures or trigger builds without switching tabs while coding.
- **Content Managers** — verify project lists and publish updates through a simple natural language prompt.
- **Designers** — keep track of project versions and page inventories via your preferred AI assistant.


## Available Tools
- **count_cms_items**: Count items in a Plasmic CMS database table
- **create_cms_item**: Create a new item in a Plasmic CMS database table
- **delete_cms_item**: Delete an item from a Plasmic CMS database table
- **get_model**: Provides a JSON representation (SDUI) of the project element tree
- **publish_cms_item**: Publish a draft item in a Plasmic CMS database table
- **query_cms_items**: Fetch items from a Plasmic CMS database table
- **render_html**: Fetches generated HTML for a specific component
- **update_cms_item**: Update an existing item in a Plasmic CMS database table
- **update_project**: Programmatically updates Plasmic projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plasmic (Visual Headless Page Builder)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Plasmic projects."

**🤖 AI Agent:**
> I've found 3 projects in your account: 'Marketing Site' (ID: 8vK...), 'E-commerce Store' (ID: 2mP...), and 'Documentation' (ID: 9qL...). Which one would you like to inspect?

---

**👤 You:**
> "Show me the pages for project ID 8vK..."

**🤖 AI Agent:**
> Fetching pages for 'Marketing Site'... I found 4 pages: 'Home' (/), 'About Us' (/about), 'Pricing' (/pricing), and 'Contact' (/contact).

---

**👤 You:**
> "Publish the latest changes for project 8vK..."

**🤖 AI Agent:**
> Publishing 'Marketing Site' (ID: 8vK...) now... The project has been successfully published to production.


## ❓ FAQ

**Q: Can I list all my Plasmic projects to find a specific Project ID?**
Yes! Use the `list_projects` tool. Your agent will return a list of all projects associated with your credentials, including their names and unique IDs.

**Q: How do I see which pages are currently built inside a project?**
Simply ask the agent to run `get_project_pages` with the target Project ID. It will list all pages, their paths, and basic metadata.

**Q: Is it possible to publish my changes to production using the AI?**
Yes. By using the `publish_project` tool, you can trigger a new publish for a specific project ID, making your visual changes live immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plasmic-visual-headless-page-builder](https://vinkius.com/mcp/plasmic-visual-headless-page-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plasmic (Visual Headless Page Builder)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plasmic-visual-headless-page-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plasmic (Visual Headless Page Builder)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plasmic-visual-headless-page-builder": {
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
