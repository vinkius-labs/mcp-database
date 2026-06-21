# Sitecore MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sitecore)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sitecore-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sitecore-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Sitecore CMS via AI agents — create, search, and update content items, templates, layouts, and workflows directly from your chat.

## Description
Connect your **Sitecore** instance to any AI agent and take full control of your enterprise CMS through natural conversation. Execute headless content operations without navigating the complex Sitecore Content Editor.

### What you can do

- **Item Management** — Retrieve, create, update, and delete Sitecore items using their path or unique ID
- **Content Search** — Search deeply across your content tree using keywords, templates, and dates
- **Site navigation** — List item children to traverse the content tree hierarchy natively
- **Templates & Layouts** — List available templates and retrieve presentation/layout details (renderings and placeholders) for specific pages
- **Workflows** — Check the current workflow state of any item (e.g., Draft, Review, Published)

### How it works

1. Subscribe to this server
2. Provide your Sitecore Base URL and your Services Client API Key (Item ID)
3. Start managing your digital experience platform from Claude, Cursor, or any MCP-compatible client

No more context-switching between your editor and the Sitecore backend. Your AI agent becomes your CMS copilot.

### Who is this for?

- **Content Authors** — quickly update field values across multiple pages and see their workflow states without opening the Sitecore client
- **Marketers** — rapid searches to find legacy content items or verify if specific personalized components are in the right layout
- **Developers** — automate the creation of test items and query complex Sitecore trees while coding your front-end headless applications


## Available Tools
- **create_content_item**: Requires parent ID, item name, and template ID.

Creates a new item in the Sitecore content tree
- **delete_content_item**: This action is irreversible.

Permanently deletes a Sitecore item
- **get_item_details**: Retrieves details for a specific Sitecore item
- **get_item_layout**: Retrieves the layout or presentation details for an item
- **get_workflow_state**: Retrieves the current workflow state of an item
- **list_item_children**: Lists the immediate children of a specific item
- **list_content_templates**: g., "Page", "Article") are available for creating new items.

Lists available content templates
- **search_content**: Useful for broad discovery across the CMS.

Searches for content items in Sitecore
- **update_content_item**: Provide a JSON string of field name/value pairs.

Updates the fields of an existing Sitecore item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sitecore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check the workflow state for the `/sitecore/content/Home/AboutUs` item?"

**🤖 AI Agent:**
> The item `/sitecore/content/Home/AboutUs` is currently in the **Draft** workflow state. Would you like me to get its layout presentation details as well?

---

**👤 You:**
> "List the immediate children under `/sitecore/content/Home/Products`."

**🤖 AI Agent:**
> I found 3 child items under the Products node:
1. Laptop X (ID: `110d559f...`, Template: ProductPage)
2. Monitor Y (ID: `220a3...`, Template: ProductPage)
3. Keyboard Z (ID: `330b...`, Template: ProductPage)

Which item would you like me to fetch full details for?

---

**👤 You:**
> "Create a new item named 'SpringCampaign' using template `5F22...` under parent ID `3D66...`."

**🤖 AI Agent:**
> The item **'SpringCampaign'** has been successfully created. 
New Item ID: `{A1B2C3D4-E5F6-0000...}`.
Path: `/sitecore/content/Home/Campaigns/SpringCampaign`.
Would you like me to update its initial fields with a specific JSON object?


## Installation & Usage

To install and use the **Sitecore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sitecore](https://vinkius.com/mcp/sitecore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
