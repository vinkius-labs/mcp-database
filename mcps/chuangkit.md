# Chuangkit / 创客贴 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chuangkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Leading graphic design platform in China — manage templates, materials, and designs via AI.

## Description
Empower your AI agent to orchestrate your creative workflows with **Chuangkit** (创客贴), the premier graphic design platform in China. By connecting Chuangkit to your agent, you transform complex template searching, design auditing, and material management into a natural conversation. Your agent can instantly list design templates, retrieve detailed structure for your creations, search for specific visual assets, and even provide status updates for your application without you ever needing to navigate the comprehensive Chuangkit web interface. Whether you are conducting a brand consistency audit or monitoring creative production, your agent acts as a real-time creative assistant, keeping your visual data accurate and your production moving.

### What you can do

- **Creative Orchestration** — List and retrieve detailed information about your design templates and creative projects.
- **Asset Management** — Browse materials, fonts, and visual assets to identify resources for your next project.
- **Design Tracking** — List and retrieve detailed metadata for user-created designs to monitor production progress.
- **Search & Discovery** — Use natural language to search for specific templates and categories matching your keywords.
- **Application Insights** — Retrieve high-level information about your Chuangkit application status and metadata.

### How it works

1. Subscribe to this server
2. Enter your Chuangkit App ID and App Secret
3. Start managing your creative assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor creative output and audit template consistency through natural language queries.
- **Design Leads** — coordinate asset usage and browse project structures directly from your AI-powered workspace.
- **Operations Teams** — oversee creative production and retrieve application metadata via a unified AI interface.
- **Chuangkit Power Users** — integrate your existing design workflows into your AI-driven daily routines.


## Available Tools (8)
- **get_asset_url**: Get asset download URL
- **get_design_detail**: Get user design detail
- **get_template**: Get template details
- **list_categories**: List template categories
- **list_materials**: ).

List design materials
- **list_templates**: List design templates
- **list_user_designs**: List user designs
- **search_templates**: Search templates by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chuangkit / 创客贴** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Summer Sale' design templates in Chuangkit."

**🤖 AI Agent:**
> I've retrieved several 'Summer Sale' templates for you. You have options for social media posts, banners, and posters. Which category would you like to explore further?

---

**👤 You:**
> "Show me all my recent designs."

**🤖 AI Agent:**
> I've listed your recent Chuangkit designs. You have 5 projects in progress, including 'Annual Report 2026' and 'Product Catalog'. Would you like to see the details for any of them?

---

**👤 You:**
> "List all available design categories."

**🤖 AI Agent:**
> I've retrieved the design categories from Chuangkit. There are 12 primary categories, including 'Business Cards', 'Social Media', 'Presentations', and 'Marketing Materials'. Which one fits your needs?


## ❓ FAQ

**Q: How do I find my Chuangkit App ID and Secret?**
Log in to the [Chuangkit Open Platform](https://open.chuangkit.com/), create a new application, and you will find your App ID and App Secret in the application credentials section.

**Q: Can I retrieve the download URL for an asset?**
Yes. Use the `get_asset_url` tool with the specific asset ID. Your agent will retrieve the actual URL where the resource can be accessed or downloaded.

**Q: Is it possible to search for templates by keyword?**
Yes! Use the `search_templates` tool with your desired keyword. Your agent will return a list of matching templates categorized by their visual type and usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chuangkit](https://vinkius.com/mcp/chuangkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chuangkit / 创客贴** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chuangkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chuangkit / 创客贴** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chuangkit": {
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
