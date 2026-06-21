# GatherContent MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gathercontent)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage structured content projects, track items, and oversee workflows via AI agents with GatherContent.

## Description
Connect your **GatherContent** (by Bynder) account to any AI agent to automate your structured content operations and editorial workflows through the Model Context Protocol (MCP). GatherContent is a content operations platform that helps teams organize and produce structured content at scale. This MCP server enables you to manage your content projects, retrieve item data, and track workflow statuses directly through natural conversation.

### Key Features

- **Project Orchestration** — List all content projects and fetch detailed configuration metadata for each environment.
- **Content Oversight** — Access and retrieve structured data from your content items (pages, articles), including field-level metadata.
- **Workflow Automation** — Monitor and list the workflow statuses (e.g., Draft, Review, Published) configured for your projects.
- **Item Management** — Programmatically create new content items or update existing ones to keep your production pipeline moving.
- **Template Discovery** — Access available content templates and fetch field schemas to ensure consistent data entry.
- **Folder Navigation** — List project folders to understand your content hierarchy and organization.
- **User Identity** — Fetch profile information for the authenticated API identity to verify access levels.
- **Real-time Synchronization** — Keep your structured content strategy accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GatherContent Email and API Key (found in Personal Settings > API)
3. Start managing your content production from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Strategists & Editors** — quickly check item statuses or fetch structured content without manual exports.
- **Project Managers** — get a real-time overview of content production across multiple projects via simple AI commands.
- **Operations Teams** — automate the creation of placeholder items and verify template schemas seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **create_content_item**: Create new item
- **get_item_content**: Get item metadata/content
- **get_my_identity**: Get current user profile
- **get_project_details**: Get project metadata
- **get_template_schema**: Get template fields
- **list_project_folders**: List project folders
- **list_project_items**: List content items
- **list_content_projects**: List all projects
- **list_content_templates**: List project templates
- **list_workflow_statuses**: ) for a project.

List workflow states
- **update_content_item**: Modify item metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GatherContent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active content projects in my account."

**🤖 AI Agent:**
> Retrieving projects... I found 3 active projects: 'Website Redesign', 'Blog Production', and '2024 Product Guide'. Which project would you like to explore?

---

**👤 You:**
> "Show me the content items in the 'Blog Production' project (ID: 12345)."

**🤖 AI Agent:**
> Fetching items... I found 12 items in 'Blog Production'. Key items include '10 Tips for Content Strategy' (Status: Review) and 'What is MCP?' (Status: Draft).

---

**👤 You:**
> "Get the field values for item 'item_98765'."

**🤖 AI Agent:**
> Retrieving item content... For item 98765, I found fields for 'Headline', 'Body Copy', and 'Meta Description'. The body copy currently contains 450 words and is marked as 'Ready for Review'.


## ❓ FAQ

**Q: How do I get an API Key for GatherContent?**
Log in to your GatherContent account, click on your profile avatar, navigate to Personal Settings > API, and you can generate a new API Key there.

**Q: What email should I use for authentication?**
You must use the exact email address associated with your GatherContent user account. This email is used as the username for Basic Authentication.

**Q: Can I see the structured fields of a content item?**
Yes! The 'get_item_content' tool retrieves the full metadata and content for any item, including the specific data values stored in each defined field.

**Q: How do I find my Project ID?**
You can use the 'list_content_projects' tool to see all your active projects and their corresponding IDs, or look at the URL when you are viewing a project in your browser.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gathercontent](https://vinkius.com/mcp/gathercontent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GatherContent** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gathercontent` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GatherContent** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gathercontent": {
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
