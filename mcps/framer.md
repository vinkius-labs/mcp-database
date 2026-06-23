# Framer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/framer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Equip your AI agent with direct access to Framer — manage CMS collections, sync content, and publish site changes without opening the Framer editor.

## Description
Connect **Framer** to your AI agent and manage your website CMS content and publishing workflow conversationally.

### What you can do

- **CMS Collections** — List, create, update, and manage CMS collection items directly from natural language commands.
- **Content Sync** — Push content updates from external data sources into your Framer CMS collections programmatically.
- **Site Publishing** — Trigger site publishes to push your latest CMS changes live.
- **Collection Schema** — Query collection structures and field definitions to understand your content model.

### How it works

1. Subscribe to the Framer integration on the marketplace.
2. Generate a Server API key from your Framer project (Site Settings → General → generate API key).
3. Ask your AI agent to manage CMS content, sync data, or publish your site.

### Who is this for?

- **Design-Led Teams** — Update website content without touching the Framer canvas or disrupting design layouts.
- **Marketing Teams** — Publish landing pages, blog posts, and campaign content directly from conversations.
- **Developers** — Programmatically sync CMS data from headless APIs, databases, or spreadsheets into Framer.


## Available Tools (8)
- **list_projects**: List all Framer projects
- **get_project**: Get project details
- **list_collections**: List CMS collections
- **list_collection_items**: List items in a CMS collection
- **create_collection_item**: Create a new CMS item
- **publish_site**: This makes changes visible to visitors.

Publish the website
- **list_pages**: List all site pages
- **get_site_info**: Get site configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Framer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all CMS collections in my Framer site."

**🤖 AI Agent:**
> Your Framer project has 3 CMS collections: 'Blog Posts' (18 items), 'Team Members' (12 items), and 'Case Studies' (7 items).

---

**👤 You:**
> "Add a new team member 'Ana Silva' to the Team Members collection."

**🤖 AI Agent:**
> Team member 'Ana Silva' added to the 'Team Members' collection. Fields set: Name, Role (empty). You can ask me to update additional fields like bio, photo URL, or social links.

---

**👤 You:**
> "Publish my Framer site with the latest CMS changes."

**🤖 AI Agent:**
> Site publish triggered. Your CMS changes are now live. Last updated: just now. All 37 collection items synced across 3 collections.


## ❓ FAQ

**Q: How do I get my Framer API key?**
Open your Framer project in the editor. Go to **Site Settings** (gear icon in the top bar), then navigate to the **General** tab. Scroll down to find the **Server API** section and click **Generate API key**. Copy the key and store it securely — treat it like a password. This key is specific to this project. Paste it into the configuration field below.

**Q: Can I push content from a spreadsheet into my Framer CMS?**
Yes. Your AI agent can create and update CMS collection items programmatically. Describe the data you want to add, and it maps your fields to the Framer collection schema and creates the items — perfect for bulk content migrations or data-driven landing pages.

**Q: Does publishing through the API affect my Framer design?**
No. The Server API only manages CMS content — it cannot modify your visual design, canvas layout, or component structure. Your designers remain in full control of the visual experience while content teams operate independently through the AI agent.

**Q: Is this suitable for agencies managing multiple Framer projects?**
Yes. Each API key is bound to a specific Framer project. Configure separate integrations for each client project and your AI agent can switch between them — managing content across your entire portfolio without opening multiple browser tabs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/framer](https://vinkius.com/mcp/framer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Framer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `framer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Framer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "framer": {
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
