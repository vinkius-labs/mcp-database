# Webflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webflow-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Design and build professional websites visually with a no-code platform that generates clean, production-ready HTML and CSS.

## Description
Connect your **Webflow** account to any AI agent and simplify how you manage your web projects, dynamic content, and e-commerce operations through natural conversation.

### What you can do

- **Site Management** — List all your Webflow sites and retrieve detailed metadata and status updates.
- **CMS Operations** — Query CMS collections and list items to manage dynamic content without opening the Designer.
- **E-commerce Tracking** — Monitor your online store by listing and inspecting recent orders and customer data.
- **Asset Management** — List uploaded assets like images and files to keep track of your site's media library.
- **User Coordination** — Manage registered site users and memberships directly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Webflow API Access Token (found in your site or workspace settings)
3. Start managing your web ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Web Developers** — quickly verify CMS data and inspect site configurations during the build process.
- **Content Managers** — list and update CMS items or verify asset availability via simple AI queries.
- **Store Owners** — monitor e-commerce orders and customer growth directly from the workspace.


## Available Tools
- **create_collection_item**: Create a new CMS item
- **get_site_details**: Get details for a specific site
- **list_site_assets**: List uploaded site assets
- **list_cms_collections**: List CMS collections for a site
- **list_collection_items**: List items in a CMS collection
- **list_ecommerce_orders**: List e-commerce orders
- **list_sites**: List all Webflow sites
- **list_site_users**: List registered site users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Webflow sites."

**🤖 AI Agent:**
> I've retrieved your sites. You have access to: 'Portfolio 2024', 'Company Dashboard', and 'Marketing Landing Page'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the items in the 'Blog Posts' collection for site 'site_12903'."

**🤖 AI Agent:**
> I've fetched the items from 'Blog Posts'. There are 5 entries including 'Intro to AI', 'Webflow Tips', and 'Case Study: Vinkius'. Would you like details on any specific post?

---

**👤 You:**
> "Check for any new e-commerce orders on site 'site_12903'."

**🤖 AI Agent:**
> Inspecting recent orders... I found 2 new orders: #ORD-552 ($120.00) and #ORD-553 ($45.50). Both are marked as 'Processing'. Shall I retrieve the customer details?


## ❓ FAQ

**Q: Can I see my e-commerce orders using the AI?**
Yes! Use the `list_ecommerce_orders` tool with your Site ID. Your agent will retrieve all recent orders processed in your Webflow store.

**Q: How do I add a new item to my blog collection?**
Use the `create_collection_item` action. Provide the Collection ID and a JSON object with the field values for your new blog post.

**Q: Is it possible to list all images uploaded to a site?**
Absolutely. Use the `list_site_assets` query to retrieve a complete list of uploaded images, files, and media available in your site's library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webflow-alternative](https://vinkius.com/mcp/webflow-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Webflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `webflow-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Webflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webflow-alternative": {
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
